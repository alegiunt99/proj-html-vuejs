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
                      <span v-if="index === 0"><strong>$62 For 2 Hours</strong> - Lorem ipsum salem irides</span>
                  </div>
                  
              </div>
          </div>
      </div>
  </section>
</template>

<script>

import offersToBuy from '@/offersToBuy.json'

export default {
  name: 'FaceAndBody',

  data(){
      return {
          offersBoxes: offersToBuy,
      }
  },
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
    }
}

section{
    background-color: gainsboro;
}
//face_and_body_treatments-new.jpg

</style>