<template>
  <header>
    <div class="container">

      <a href="/">
        <img src="../assets/img/dc-logo.png" alt="logo dc">
      </a>

      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :class="{'active': link.current}" :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </nav>

    </div>
  </header>
</template>

<script>

export default {
  name: 'HeaderComp',
  data(){
    return{
      links:[
        {
          text: 'characters',
          url: '/',
          current: false
        },
        {
          text: 'comics',
          url: '/',
          current: true
        },
        {
          text: 'movies',
          url: '/',
          current: false
        },
        {
          text: 'tv',
          url: '/',
          current: false
        },
        {
          text: 'games',
          url: '/',
          current: false
        },
        {
          text: 'collectibles',
          url: '/',
          current: false
        },
        {
          text: 'videos',
          url: '/',
          current: false
        },
        {
          text: 'fans',
          url: '/',
          current: false
        },
        {
          text: 'news',
          url: '/',
          current: false
        },
        {
          text: 'shop',
          url: '/',
          current: false
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

  @import '../assets/style/vars.scss';
  
  h2{
    color: $brand-color;
  }
  
  img{
    height: 80px;
  }

  .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: #1C1C1C;
    height: 100%;
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
