<template>
  <div id="app">
    <!-- header -->
    <HeaderCom/>

    <!-- main -->
    <MainCom/>

    <!-- footer -->
    <FooterCom/>
  </div>
</template>

<script>
import HeaderCom from './components/HeaderCom.vue';
import MainCom from './components/MainCom.vue';
import FooterCom from './components/FooterCom.vue'

export default {
  name: 'App',
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

</style>
