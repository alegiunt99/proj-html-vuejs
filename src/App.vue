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
</style>
