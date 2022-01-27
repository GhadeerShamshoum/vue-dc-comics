<template>
  <div>
    <footer> 
      <div>
        <div class="footerBottom">
            <div class="container B">
            <button>sign-up now!</button>
            <div class="bottomRight">follow us
                <img class="icons" src="../assets/img/footer-facebook.png" alt="">
                <img class="icons" src="../assets/img/footer-twitter.png" alt="">
                <img class="icons" src="../assets/img/footer-youtube.png" alt="">
                <img class="icons" src="../assets/img/footer-pinterest.png" alt="">
                <img class="icons" src="../assets/img/footer-periscope.png" alt="">
            </div>
            </div>
        </div>
      </div>
    </footer>   
  </div>
</template>

<script>


export default {
  name: 'FooterBottom',
   
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/partials/variables.scss';

.footerBottom{
  height: 100px;
  background-color: rgb(51, 50, 50);
  color: $colorBlue;
  display: flex;
  justify-content: space-between;
  align-items: center;
  text-transform: uppercase;
  button{
    height: 50px;
    width: 180px;
    font-size: 20px;
    text-transform: uppercase;
    border: 2px solid $colorBlue;
    background-color: transparent;
    color: white;

  }
  .bottomRight{
    line-height: 100px;
    display: flex;
    align-items: center;


    .icons{
      padding:0 10px;
    }
  }
}

.container.B{
  display: flex;
  justify-content: space-between;
  align-items: center;

}



</style>
