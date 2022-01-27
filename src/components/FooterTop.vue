<template>
  <div>
    <footer>
      <div class="footerTop">
        <div class="container">
          <div class="foterTopContainer" v-for='(element, index) in information' :key="index">
            <img src="../assets/img/img_1.png" alt="">
            <div class="text">{{element.text}}</div>
          </div>
        </div>
      </div>
    </footer>   
  </div>
</template>

<script>
export default {
  name: 'FooterTop',
   data (){
    return{
      information:[
        {
          text: "digital comics",
          image:"../assets/img/img_1.png"
        },
        {
          text: "dc merchandise",
          image:"../assets/img/img_2.png"
        },
        {
          text: "subscription",
          image:"../assets/img/img_3.png"
        },
        {
          text: "comic shop locator",
          image:"../assets/img/img_4.png"
        },
        {
          text: "dc power visa"
          
        }
        
      ]
    }
  }
  
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/partials/variables.scss';


.container{
  display: flex;
  justify-content: space-around;
  align-items: center;

}
.footerTop{
  background-color: $colorBlue;
  height: 150px;
  width: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  .foterTopContainer{
    display: flex;
    align-items: center;
    
    img{
      height: 60px;
    }
    .text{
      padding: 0 5px;
      
    }
  }
}




footer{
  background-image: url(../assets/img//footer-bg.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}



</style>
