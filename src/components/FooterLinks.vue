<template>
  <section class="links">
    <div class="container">

      <!-- colonna 1 -->
      <div>
        <ul>
          <li><a href="#">DC COMICS</a></li>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
        </ul>

        <ul>
          <li><a href="#">SHOP</a></li>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectabilities</a></li>
        </ul>

      </div>
      <!-- /colonna 1 -->

      <!-- colonna 2 -->
      <div>
        <ul>
          <li><a href="#">DC</a></li>
          <li><a href="#">Terms Of Use</a></li>
          <li><a href="#">Privacy policy(New)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </div>
      <!-- /colonna 2 -->

      <!-- colonna 3 -->
      <div>
        <ul>
          <li><a href="#">SITES</a></li>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>
      <!-- /colonna 3 -->

    </div>
  </section>
</template>

<script>
export default {
  name: 'FooterLinks'
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/vars.scss';
  @import '../assets/style/mixin.scss';

  section.links{
    background-image: url('../assets/img/footer-bg.jpg');
    overflow: hidden;
    .container{
      display: flex;
      position: relative;
      background-image: url('../assets/img/dc-logo-bg.png');
      background-repeat: no-repeat;
      background-size: 320px;
      background-position: right center;
      div{
        flex-basis: calc(100% / 10);
        padding: 30px 10px 30px 0;
      }
    }
  }

  ul{
    li:first-child{
      font-size: 0.6rem;
      font-weight: 600;
      margin-bottom: 10px;
      a{
        color: white;
      }
    }
    li{
      font-size: 0.5rem;
      margin: 6px 0;
      a{
        color: #6D7364;
      }
    }
    li:last-child{
      margin-bottom: 10px;
    }
  }


</style>