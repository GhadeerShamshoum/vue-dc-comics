<template>
  <div>
    <footer>
      <div class="footerTop">
        <div class="container">
          <div class="foterTopContainer" v-for='(element, index) in information' :key="index">
              <div class="imgContainer">
                <img :src="element.image" alt="">
              </div>
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
          image:require("../../assets/img/img_1.png")
        },
        {
          text: "dc merchandise",
          image:require("../../assets/img/img_2.png")
        },
        {
          text: "subscription",
          image:require("../../assets/img/img_3.png")
        },
        {
          text: "comic shop locator",
          image:require("../../assets/img/img_4.png")
        },
        {
          text: "dc power visa",
          image:require("../../assets/img/img_5.svg")
          
        }
        
      ]
    }
  }
  
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../../assets/style/partials/variables.scss';


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
    .imgContainer{
        width: 60px;
        height: 50px;
        img{
          height: 100%;
        }
    }
    
    .text{
      padding: 0 5px;
      
    }
  }
}




footer{
  background-image: url(../../assets/img/footer-bg.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}



</style>
