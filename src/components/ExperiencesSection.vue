<template>
  <section>
    <div class="container">
      <h2>Luxury SPA Experiences</h2>
      <i class="fa-solid fa-leaf"></i>
      <p>gray</p>
      <div>___</div>
      <span>story</span>
      <button>click here</button>
      <div class="exp-buttons-list">

        <div v-for="(item, index) in exButtons" :key="index" :class="`ex-btn-${item.classType}`">
          <i :class="['fa-solid', `fa-${item.iconName}`]"></i>
          <p>{{item.text}}</p>
        </div>

      </div>

    </div>
  </section>
</template>

<script>

import experiencesButton from '@/experiencesButtons.json';

export default {
  name: 'ExperiencesSection',
  
  data(){
    return {
      exButtons: experiencesButton,
    }
  },
}
</script>


<style scoped lang="scss">

.container{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  row-gap: 10px;
  .exp-buttons-list{
    display: flex;
    column-gap: 91px;
    margin-top: 20px;
    width: 100%;
    padding-left: 50px;
    justify-content: center;
    .ex-btn-top{
      padding-bottom: 10px
    }
    .ex-btn-bottom{
      padding-top: 35px
    }
    i{
      font-size: 32px;
      margin-bottom: 10px;
    }
    p{
      font-size: 15px;
    }
  }
}

</style>