<template>
  <footer>

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

        <img src="../assets/img/dc-logo-bg.png" alt="dc logo">

      </div>
    </section>
    
    <section class="social">
      <div class="container">

        <div><button>SIGN-UP NOW!</button></div>

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

  </footer>
</template>

<script>

export default {
  name: 'FooterComp',
  /* data(){
    
  } */
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/vars.scss';

  footer{
    section.links{
      background-image: url('../assets/img/footer-bg.jpg');
      padding: 30px 0;
      overflow: hidden;
      .container{
        display: flex;
        position: relative;
        div{
          flex-basis: calc(100% / 10);
          padding-right: 10px;
        }
        img{
          position: absolute;
          top: -90px;
          right: 80px;
          height: 350px;
        }
      }
    }
    section.social{
      min-height: 110px;
      .container{
        display: flex;
        justify-content: space-between;
        div{
          line-height: 110px;    
        }
      }
    }
  }

  section.links ul{
    li:first-child{
      font-size: 0.6rem;
      font-weight: 600;
      margin-bottom: 10px;
      a{
        color: white;
      }
    }
    li{
      font-size: 0.4rem;
      margin: 6px 0;
      a{
        color: #6D7364;
      }
    }
    li:last-child{
      margin-bottom: 10px;
    }
  }

  section.social ul{
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