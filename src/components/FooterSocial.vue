<template>
  <section class="social">
    <div class="container">

      <div>
        <button>SIGN-UP NOW!</button>
      </div>

      <div>
        <ul>
          <li><a href="#">FOLLOW US</a></li>
          <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a></li>
          <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a></li>
          <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a></li>
          <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a></li>
          <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="eriscope"></a></li>
        </ul>
      </div>

    </div>
  
  </section>
</template>

<script>
export default {
  name: "FooterSocial"
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/general.scss';
  @import '../assets/style/utilities.scss';
  @import '../assets/style/vars.scss';
  @import '../assets/style/mixin.scss';


  section.social{
    height: 110px;
    .container{
      @include center('vertical');
    }
  }

  ul{
    li:first-child{
      font-weight: 600;
      margin-right: 10px;
    }
    li{
      display: inline-block;
      margin: 0 5px;
      a{
        color: $brand-color;
        font-size: 0.8rem;
        img{
          height: 25px;
          vertical-align: middle;
        }
      }
    }
  }

  button{
    border: 2px solid $brand-color;
    padding: 10px;
    font-size: 0.6rem;
    background: transparent;
    color: white;
  }

</style>