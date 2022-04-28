<template>
  <div id="app">
    <!-- header -->
    <HeaderCom :menu="menu"/>

    <!-- main -->
    <MainCom :exButtons="experiencesButton" :cards="treatsCards" :offersBoxes="offersToBuy"/>

    <!-- footer -->
    <FooterCom :links="footerLinks"/>
  </div>
</template>

<script>
// components
import HeaderCom from './components/HeaderCom.vue';
import MainCom from './components/MainCom.vue';
import FooterCom from './components/FooterCom.vue'

// json
import headerMenu from '@/headerMenu.json';

import experiencesButton from '@/experiencesButtons.json';
import offersToBuy from '@/offersToBuy.json';
import treatsCards from '@/treatsCards.json'

import footerLinks from '@/footerLinks.json'

export default {
  name: 'App',

  data(){
    return{
      footerLinks,

      menu: headerMenu,

      experiencesButton,

      treatsCards,

      offersToBuy

    }
  },
  components: {

    HeaderCom,

    MainCom,

    FooterCom,
  }
}
</script>

<style lang="scss">

*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.container{
  width: 85%;
  margin: 0 auto;
}

h1{
  font-size: 66px;
}

h2{
  font-size: 53px;
}

/* :cards="treatsCards" :offersBoxes="offersToBuy"*/

</style>
