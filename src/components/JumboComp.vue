<template>
  <section>
    <div class="container">
      <button class="btn-brand">CURRENT SERIES</button>
    </div>
  </section>
</template>

<script>
export default {
  name: 'JumboComp',
}
</script>

<style lang="scss" scoped>

  section{
    height: 400px;
    background-image: url('../assets/img/jumbotron.jpg');
    background-size: cover;
    .container{
      position: relative;
      button{
        font-size: 1.5rem;
        position: absolute;
        bottom: -10px;
        padding: 5px 15px;
        font-weight: 600;
      }
    }

  }
</style>