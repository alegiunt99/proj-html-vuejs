<template>
  <main>
      <h1>main</h1>
      <!-- Jumbotron -->
      <JumbotronSection/>
      
      <!-- sezione delle esperienze -->
      <ExperiencesSection/>
      
      <!-- sezione dei trattamenti -->
      <TreatmentsSection/>
      
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