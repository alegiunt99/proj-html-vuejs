<template>
  <header>
    <div v-for="(item, index) in menu" :key="index">
      <p>{{item.primaryText}}</p>
    </div>
  </header>
</template>

<script>
import headerMenu from '@/headerMenu.json'

export default {
  name: 'HeaderCom',

  data(){
    return {

      menu: headerMenu,

    }
  },

  methods: {
    showMenu(){
      console.log(this.menu)
    }
  }
}
</script>


<style scoped lang="scss">

</style>