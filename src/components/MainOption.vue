<template>
  <section>
    <div class="container">

      <div>
        <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
        <p>digital comics</p>
      </div>

      <div>
        <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise">
        <p>merchandise</p>
      </div>

      <div>
        <img src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
        <p>subscription</p>
      </div>

      <div>
        <img src="../assets/img/buy-comics-shop-locator.png" alt="comic shop locator">
        <p>comic shop locator</p>
      </div>

      <div>
        <img src="../assets/img/buy-dc-power-visa.svg" alt="dc power visa">
        <p>dc power visa</p>
      </div>

    </div>
  </section>
</template>

<script>

export default {
  name: 'MainOption'
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/vars.scss';
  @import '../assets/style/mixin.scss';

  section{
    height: 150px;
    background-color: $brand-color;
  }

  .container{
    display: flex;
    div{
      flex-basis: calc(100% / 5);
      position: relative;
      text-align: center;
      line-height: 150px;
      img{
        max-width: 55px;
        max-height: 60px;
        transform: translateY(30%);
      }
      p{
        display: inline-block;
        margin-left: 10px;
        font-size: 0.8rem;
        text-transform: uppercase;
      }
    }
  }


</style>