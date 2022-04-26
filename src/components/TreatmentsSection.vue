<template>
  <section>
    <!-- face & body treatment -->
    <FaceAndBody/>

    <!-- our treatment -->
    <OurTreatments />

  </section>
</template>

<script>

import FaceAndBody from '@/components/FaceAndBody.vue';
import OurTreatments from '@/components/OurTreatments.vue';

export default {
  name: 'TreatmentsSection',

  components:{

    FaceAndBody,

    OurTreatments

  }
}
</script>


<style scoped lang="scss">

</style>