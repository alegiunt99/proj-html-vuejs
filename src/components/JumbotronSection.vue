<template>
  <section class="jumbotron">
    <div class="container">
      <span>lorem</span>

      <h1>jumbo</h1>

      <button>acquista</button>

      <div>
        <span>demos</span>
      </div>

      <div>
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
  }
}
</style>