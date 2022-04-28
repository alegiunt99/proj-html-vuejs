<template>
  <section>
    <div id="title">
      <h2>OUR TREATMENTS</h2>
    </div>

    <div>
      <TreatmentCard :cards="treatCards"/>
    </div>
  </section>
</template>

<script>7
import TreatmentCard from '@/components/TreatmentCard.vue'

//import treatsCards from '@/treatsCards.json'

export default {
  name: 'OurTreatments',

  data(){
    return{
      treatCards: this.cards,
    }
  },

  props:{

    cards: Array,

  },

  components: {
    TreatmentCard,
  }
}
</script>


<style scoped lang="scss">

</style>