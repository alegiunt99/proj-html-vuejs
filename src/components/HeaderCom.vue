<template>
  <header >

    <div class="container">
        <div class="row">

        <div class="d-flex align-items-cent">
          <i class="fa-solid fa-home"></i>
        </div>

        <div class="header-link">
          <i :class="['fa-solid', `fa-${menu[0].iconClass}`]"></i>
          <p>{{menu[0].primaryText}}</p>
          <span>{{menu[0].subText}}</span>
          <span></span>
        </div>

        <div class="header-link">
          <i :class="['fa-solid', `fa-${menu[1].iconClass}`]"></i>
          <p>{{menu[1].primaryText}}</p>
          <span>{{menu[1].subText}}</span>
          <span></span>
        </div>

        <div id="logo-box">
          <img src="@/img/avada-spa-logo-retina-new-400x46.png" alt="LogoPrincipale">
        </div>

        <div class="header-link">
          <i :class="['fa-solid', `fa-${menu[2].iconClass}`]"></i>
          <p>{{menu[2].primaryText}}</p>
          <span>{{menu[2].subText}}</span>
          <span></span>
        </div>

        <div class="header-link">
          <i :class="['fa-solid', `fa-${menu[3].iconClass}`]"></i>
          <p>{{menu[3].primaryText}}</p>
          <span>{{menu[3].subText}}</span>
          <span></span>
        </div>

        <div class="d-flex align-items-cent">
          <i class="fa-solid fa-plus"></i>
        </div>
      </div>
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
header{
  padding: 20px 0px;
}
.container{
  .row{
    display: flex;
    justify-content: space-around;
    color:gray;
    .header-link{
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      row-gap: 8px;
      &:hover{
        color: #5db2bb;
        cursor: pointer;
      }
      p{
        margin: 0;
        font-size: 16px;
        }
      span{
        font-size: 12px;
        }
    }

    #logo-box{
      display: flex;
      flex-direction: row;
      align-items: center;
      justify-content: center;
      width: 26%;
      img{
        width: 100%;
      }
    }
  }
}



.d-flex{
  display: flex;
}

.align-items-cent{
  align-items: center;
}
</style>