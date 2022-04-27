<template>
  <div class="card">
      <div v-for="item in cards" :key="item.image_path" class="content-card">
            <div class="image-content">
                <div class="img-hover">
                    <p>{{item.title}}</p>
                </div>
                <img :src="require('@/img/layer-' + item.image_path + '-new.jpg')" class="image-default">
            </div>
            
            <h3> {{item.title}} </h3>

            <div class="separe-bar"></div>

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
}
</script>


<style scoped lang="scss">
    .card{
        display: flex;
        flex-wrap: wrap;
        .content-card{
            width: 25%;
            padding: 10px;
            border: 2px solid gainsboro;
            .image-content{
                width: 100%;
                height: 71%;
                img{
                    width: 100%;
                }
            }
            h3{
                padding-left: 10px;
            }
            .separe-bar{
                border: 1px solid gainsboro;
                width: 80%;
                margin: 20px 0;
                margin-left: 10px;
            }
            p{
                padding-left: 10px;
                font-size: 15px;
            }
            
        }
    }

    .img-hover{
        width: 100%;
        
        display:none;
    }

    .image-content:hover{
        .img-hover{
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: gray;
            color: white;
            margin-bottom: 4px;
        }
        .image-default{
            display: none;
        }

    }
</style>