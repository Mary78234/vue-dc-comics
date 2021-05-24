<template>
  <div class="box">

    <div class="box-img">
      <img :src="card.thumb" :alt="card.series">
    </div>
    <p>{{ card.series }}</p>

  </div>
</template>

<script>
export default {
  name: 'ProductComp',
  props:{
    card: Object
  }
}
</script>

<style  lang="scss" scoped>

  div.box{
    flex-basis: calc(100% / 6);
    margin: 20px 0;
    padding: 0 10px;
    .box-img{
      position: relative;
      height: 160px;
      overflow: hidden;
      img{
        position: absolute;
        top: 0;
        width: 100%;
      }
    }
    p{
      text-transform: uppercase;
      margin: 15px 0;
      font-size: 0.8rem;
    }
  }



</style>