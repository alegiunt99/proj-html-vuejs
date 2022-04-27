<template>
  <footer>
    <div class="container">
      <!-- logo -->
      <div>
        <img src="@/img/avada-spa-logo-retina-new-200x23.png" alt="logo">
      </div>

      <!-- links e copyright -->
      <div class="copiryght-links">
        <div v-for="(item, index) in links" :key="index" >
          <a href="#">{{item.credit}}</a>
        </div>
      </div>

      <!-- link ai social network -->
      <div class="social-networks">
        <div v-for="(item, index) in links" :key="index" >
          <i :class="['fa-brands', `fa-${item.social}`]"></i>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterCom',

  props:{
    links: Array
  },
}
</script>


<style scoped lang="scss">
footer{
  padding: 30px 0px;
  .container{
    display: flex;
    align-items: center;
    justify-content: space-between;
    .copiryght-links{
      display: flex;
      justify-content: center;
      font-size: 13px;
      flex-wrap: wrap;
      & > *{
        width: 33%;
        a{
          color: gray;
          text-decoration: none;
          &:hover{
            color: rgb(6, 114, 255);
          } 
        }
      }
    }
    .social-networks{
      display: flex;
      column-gap: 18px;
      color: gray;
      font-size: 15px;
      & > *{
        background-color: lightgrey;
        padding: 8px;
      }
    }
  }
}
</style>