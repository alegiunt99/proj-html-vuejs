<template>
  <section>
    <div id="title">
      <h2>OUR TREATMENTS</h2>
    </div>

    <div>
      <TreatmentCard :cards="cards"/>
    </div>
  </section>
</template>

<script>7
import TreatmentCard from '@/components/TreatmentCard.vue'

import treatsCards from '@/treatsCards.json'

export default {
  name: 'OurTreatments',

  data(){
    return {
      cards: treatsCards,
    }
  },

  components: {
    TreatmentCard,
  }
}
</script>


<style scoped lang="scss">

</style>