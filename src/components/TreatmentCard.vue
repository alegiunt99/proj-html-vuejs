<template>
  <div class="card">
      <div v-for="item in cards" :key="item.image_path" >
            <img :src="`@/img/Layer-${item.image_path}-new.jpg`" :alt="item.title">
            <h3> {{item.title}} </h3>
            <div></div>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Cum aliquam laborum tempore, illum maxime repellendus! Quia corporis amet vitae eos!</p>
      </div>
      
  </div>
</template>

<script>
export default {
  name: 'TreatmentCard',

  props:{
      cards: Array,
  }
}
</script>


<style scoped lang="scss">

</style>