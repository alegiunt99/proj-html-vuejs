<template>
  <div class="card">
      <div v-for="item in cards" :key="item.image_path" class="content-card">
            <img :src="require('@/img/layer-' + item.image_path + '-new.jpg')">
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
  },

  methods: {
      imgUrl(item){

          const url = `@/img/layer-${item.image_path}-new.jpg`;

          return url;

      }
  }
}
</script>


<style scoped lang="scss">
    .card{
        display: flex;
        flex-wrap: wrap;
        .content-card{
            width: 25%;
            img{
                width: 100%;
            }
        }
    }
</style>