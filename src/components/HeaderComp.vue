<template>
  <header>
    <div class="container">

      <a href="/">
        <img src="../assets/img/dc-logo.png" alt="logo dc">
      </a>

      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :class="(index === positionActive) ? 'active' : null" 
              :href="link.url"
              @click="positionActive = index"
            >{{ link.text }}</a>
          </li>
        </ul>
      </nav>

    </div>
  </header>
</template>

<script>
import links from '../assets/data/links.js';

export default {
  name: 'HeaderComp',
  data(){
    return{
      positionActive: 0,
      links
    }
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/vars.scss';
  @import '../assets/style/mixin.scss';
  
  h2{
    color: $brand-color;
  }
  
  img{
    height: 80px;
  }

  .container{
    @include center('vertical');
    color: #1C1C1C;
  }

  ul{
    li{
      display: inline;
        padding: 10px;
      a{
        display: inline-block;
        color: #303030;
        line-height: 96px;
        font-size: 0.6rem;
        font-weight: 600;
        text-transform: uppercase;
        &:hover,
        &.active{
          color: $brand-color;
          border-bottom: 4px solid $brand-color;
        }
      }
    }
  }


</style>
