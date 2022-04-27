<template>
  <section>
    <div class="container">
      <h2>Luxury SPA Experiences</h2>
      <i class="fa-solid fa-leaf text-gray"></i>
      <p class="text-gray">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. 
        Excepturi, reiciendis velit. Quidem commodi 
        aut perspiciatis ratione.
      </p>
      <div id="separe-bar"></div>
      <span class="text-gray">
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
        Perferendis eveniet itaque voluptate debitis mollitia assumenda
        laborum laudantium nisi, ullam, minus ea quibusdam harum dicta. 
        Eaque temporibus, optio qui nostrum, voluptate nobis obcaecati 
        veritatis, ducimus nulla quidem reiciendis ipsa debitis ullam!
      </span>
      <button>OUR APPROACH</button>
      <div class="exp-buttons-list">

        <div v-for="(item, index) in exButtons" :key="index" :class="`ex-btn-${item.classType} text-gray`" >
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
  padding: 0 160px;
  #separe-bar{
    border: 1px solid rgb(151, 151, 151);
    width: 100px;
  }
  button{
      font-size: 12px;
      padding: 8px 20px;
      border-radius: 15px;
      background-color: white;
      border: 1px solid #4c4c4c;
      color: #4c4c4c;
      &:hover{
        color: #5db2bb;
        border-color: #5db2bb;

        cursor: pointer;
      }
    }
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

section{
  margin-top: 50px;

  margin-bottom: 50px;
}

.text-gray{
  color: gray;
}

</style>