<template>
  <main>
    
      <!-- Jumbotron -->
      <JumbotronSection/>
      
      <!-- sezione delle esperienze -->
      <ExperiencesSection :exButtons="exercButtons"/>
      
      <!-- sezione dei trattamenti -->
      <TreatmentsSection :cards="adCards" :offersBoxes="offersBox"/>
      
      <!-- sezione della citazione -->
      <CitSection/>
      
      <!-- sezione delle offerte -->
      <OfferSection/>

  </main>
</template>

<script>

import JumbotronSection from '@/components/JumbotronSection.vue';
import ExperiencesSection from '@/components/ExperiencesSection.vue';
import TreatmentsSection from '@/components/TreatmentsSection.vue'
import CitSection from '@/components/CitSection.vue';
import OfferSection from '@/components/OfferSection.vue';

export default {
  name: 'MainCom',

  data(){
    return{
      exercButtons: this.exButtons,

      adCards: this.cards,

      offersBox: this.offersBoxes
    }
  },

  props:{
    exButtons: Array,

    cards: Array,

    offersBoxes: Array
  },

  components:{

      JumbotronSection,

      ExperiencesSection,

      TreatmentsSection,

      CitSection,

      OfferSection

  }
}
</script>


<style scoped lang="scss">

</style>