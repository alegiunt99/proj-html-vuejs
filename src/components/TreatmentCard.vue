<template>
  <div class="card">
      <div v-for="item in cards" :key="item.image_path" class="content-card">
            <div class="img-hover">
                <p>{{item.title}}</p>
            </div>
            <img :src="require('@/img/layer-' + item.image_path + '-new.jpg')" class="image-default">
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

    .img-hover{
        width: 100%;
        height: 100%;
        display:none;
    }

    .content-card:hover{
        .img-hover{
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: gray;
            color: white;
        }
        .image-default{
            display: none;
        }

    }
</style>