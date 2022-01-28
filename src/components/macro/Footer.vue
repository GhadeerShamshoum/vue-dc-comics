<template>
  <div>
    <footer>
     <FooterTop/>
     <FooterCenter/>
     <FooterBottom/>
    </footer>   
  </div>
</template>

<script>
import FooterTop from '../commons/FooterTop.vue'
import FooterCenter from '../commons/FooterCenter.vue'
import FooterBottom from '../commons/FooterBottom.vue'

export default {
  name: 'Footer',
  components: {
    FooterTop,
    FooterCenter,
    FooterBottom
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../../assets/style/partials/variables.scss';





footer{
  background-image: url(../../assets/img//footer-bg.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}



</style>
