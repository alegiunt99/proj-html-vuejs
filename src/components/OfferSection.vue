<template>
  <section>
    <div class="container">
      <div class="container-content">
        <!-- sconto in percentuale -->
        <div class="sale">
          <p>25%</p>
          <span>SPECIAL OFFER</span>
        </div>

        <!-- frase e frase 2 -->
        <div class="texts">
          <p>Take some time. Treat yourself. You deserve it.</p>
          <span>Book a treatment this month and receive a 25% on all further treatments</span>
        </div>

        <!-- button -->
        <button>BOOK NOW</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'OfferSection',
}
</script>
  
<style scoped lang="scss">
section{
  background-color: rgb(136, 133, 133);
}
.container{
 
  color: white;
  .container-content{
    display: flex;
    justify-content: space-around;
    padding: 60px 0px;
    align-items: center;
    .sale{
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 10px;
      border: 1px solid white;
      p{
        font-size: 36px;
      }
      span{
        font-size: 12px;
      }
    }
    .texts{
      display: flex;
      flex-direction: column;
      row-gap: 12px;
      p{
        font-size: 25px;
      }
      span{
        font-size: 13px;
      }
    }
    button{
      font-size: 12px;
      padding: 8px 20px;
      border-radius: 15px;
      border: none;
      color: #4c4c4c;
      &:hover{
        color: white;
        background-color: #6cd6e1;
        cursor: pointer;
      }
    }
  }
  
}
</style>