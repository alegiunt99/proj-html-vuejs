<template>
  <section class="jumbotron">
    <div class="container">
      <span id="sub-tit-jumbo">Give yourself permission</span>

      <h1>Relax, Revive and Rejuvenate</h1>

      <button>EXPLORE TREATMENTS</button>

      <div id="demos">
        <i class="fa-solid fa-clipboard-question"></i>
        <span>demos</span>
      </div>

      <div id="on-sale">
        <span id="price-sale">$39</span>
        <span>on sale</span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'JumbotronSection',
}
</script>


<style scoped lang="scss">
.jumbotron{
  background-image: url('@/img/avada-spa-slider-image-1-new.jpg');
  background-size: cover;
  padding: 233px 0px;
  background-repeat: no-repeat;  
  color: white;
  position: relative;
  .container{
    display: flex;
    flex-direction: column;
    align-items: center;
    #sub-tit-jumbo{
      font-size: 25px;
    }
    h1{
      margin: 10px 0px;
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
    #demos{
      position: absolute;
      right: 5px;
      top: 5px;
      font-size: 12px;
      background-color: gainsboro;
      color: black;
      padding: 10px;
      border-radius: 5px;
      display: flex;
      flex-direction: column;
      align-items: center;
      i{
        font-size: 22px;
      }
    }
    #on-sale{
      position: absolute;
      right: 5px;
      top: 69px;
      font-size: 12px;
      background-color: gainsboro;
      color: black;
      padding: 8px;
      border-radius: 5px;
      display: flex;
      flex-direction: column;
      align-items: center;
      #price-sale{
        font-size: 20px;
        font-weight: 600;
        color: green;
      }
    }
  }
}
</style>