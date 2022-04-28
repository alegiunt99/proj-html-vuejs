<template>
  <section>
    <!-- face & body treatment -->
    <FaceAndBody :offersBoxes="offersToBuy"/>

    <!-- our treatment -->
    <OurTreatments :cards="treatsCards"/>

  </section>
</template>

<script>

import FaceAndBody from '@/components/FaceAndBody.vue';
import OurTreatments from '@/components/OurTreatments.vue';

export default {
  name: 'TreatmentsSection',

  data(){
    return {
      treatsCards: this.cards,

      offersToBuy: this.offersBoxes
    }
  },

  props:{
    cards: Array,

    offersBoxes: Array
  },

  components:{

    FaceAndBody,

    OurTreatments

  }
}
</script>


<style scoped lang="scss">

</style>