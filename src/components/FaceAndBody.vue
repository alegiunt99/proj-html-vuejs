<template>
  <section>
      <div class="container">
          <div class="treatment-face-img">
              <img src="@/img/face_and_body_treatments-new.jpg" alt="foto trattamenti faccia e corpo">
          </div>
          <div class="buy-form">
              <h2>Face and body treatments</h2>
              <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quaerat rem ad ea rerum deserunt praesentium sed? Debitis sint error magnam.</p>
              <div class="mini-boxes-choices" v-for="(item, index) in offersBoxes" :key="index">
                  <div>
                      <i :class="['fa-solid', `fa-${item.icon}`]"></i>
                      <span> {{item.text}} </span>
                  </div>
                  <span v-if="index === 0" class="price"><strong>$62 For 2 Hours</strong> - Lorem ipsum salem irides</span>
              </div>
              <button>BOOK AN APPOINTMENT</button>
          </div>
      </div>
  </section>
</template>

<script>

//import offersToBuy from '@/offersToBuy.json'

export default {
  name: 'FaceAndBody',

  /*data(){
      return {
          offersBoxes: offersToBuy,
      }
  },*/

  props:{
      offersBoxes: Array
  }
}
</script>


<style scoped lang="scss">
.container{
    display: flex;
    padding: 90px 0px;
    column-gap: 53px;
    justify-content: center;
    .treatment-face-img{
        width: 40%;
        display: flex;
        justify-content: center;
        padding: 15px;
        border-radius: 5px;
        box-shadow: 3px 3px 5px 0px darkgrey;
        background-color: white;
        img{
            width: 100%;
        }
    }
    .buy-form{
        width: 50%;
        p{
            margin: 32px auto;
        }
        .mini-boxes-choices{
            border: 1px solid gray;
            background-color: white;
            padding: 18px;
            margin-bottom: 5px;
            display: flex;
            flex-direction: column;
            div{
                display: flex;
                align-items: center;
                column-gap: 5px;
                i{
                    font-size: 10px;
                    color: white;
                    background-color: gray;
                    padding: 4px;
                }
            }
            .price{
                padding-top: 19px;
            }
        }
        button{
            font-size: 12px;
            padding: 8px 20px;
            border-radius: 15px;
            border: 1px solid #4c4c4c;
            color: #4c4c4c;
            margin-top: 70px;
            &:hover{
                color: white;
                background-color: #6cd6e1;
                cursor: pointer;
            }
        }
    }
}

section{
    background-color: gainsboro;
}
//face_and_body_treatments-new.jpg

</style>