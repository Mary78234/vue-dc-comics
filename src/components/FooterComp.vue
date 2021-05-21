<template>
  <footer>
    
    <FooterLinks />

    <FooterSocial />

  </footer>
</template>

<script>
import FooterLinks from './FooterLinks';
import FooterSocial from './FooterSocial';

export default {
  name: 'FooterComp',
  components:{
    FooterLinks,
    FooterSocial
  }
}
</script>

<style lang="scss" scoped>

</style>