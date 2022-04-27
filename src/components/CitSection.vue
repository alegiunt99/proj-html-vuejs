<template>
  <section>
    <div class="container">
      <p>"If you want to relax, watch the clouds pass by if
        you're laying on the grass, or sit in front of creek;
        just doing nothing and having those still moments is
        what really rejuvenates the body..." </p>
      <h3>FRIEDA FRIESDSON, MASSEUSE</h3>
    </div>
  </section>
</template>

<script>
export default {
  name: 'CitSection',
}
</script>


<style scoped lang="scss">
  section{
    background-image: url('@/img/Home-quota-new.jpg');
    background-size: cover;
    background-repeat: no-repeat;
  }
  
  .container{
    padding: 219px 181px;
    text-align: center;
    color: white;
    p{
      margin-bottom: 24px;
      font-size: 24px;
      line-height: 1.8rem;
    }
    
  }
</style>