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
      <div class="container">
        <div class="footerCenter">
          <div class="containerTextFooterC">
            <div class="textContainerF">
              <h1>dc comics</h1>
              <div class="Text">
                <div>Characters</div>
                <div>Comics</div>
                <div>TV</div>
                <div>Games</div>
                <div>Videos</div>
                <div>News</div>
                <div>shop</div>
                <div>dc</div>
                <div>site</div>
              </div>
            </div>
             <div class="textContainerF">
              <h1>dc comics</h1>
              <div class="Text">
                <div>Characters</div>
                <div>Comics</div>
                <div>TV</div>
                <div>Games</div>
                <div>Videos</div>
                <div>News</div>
                <div>Shop</div>
                <div>DC</div>
                <div>Site</div>
              </div>
            </div>
             <div class="textContainerF">
              <h1>shop</h1>
              <div class="Text">
                <div>Shop DC</div>
                <div>Shop DC Collectibles</div>
              </div>
            </div>
             <div class="textContainerF">
              <h1>dc comics</h1>
              <div class="Text">
                <div>Characters</div>
                <div>Comics</div>
                <div>TV</div>
                <div>Games</div>
                <div>Videos</div>
                <div>News</div>
                <div>shop</div>
                <div>dc</div>
                <div>site</div>
              </div>
            </div>
            
          
            

          </div>
          
        </div>
      </div>
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
  name: 'Footer',
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

.footerCenter{
  height: 500px;
  width: 100%;
  background-image:url(../assets/img/dc-logo-bg.png);
  background-position: right;
  background-repeat: no-repeat;
  .containerTextFooterC{
    margin: 60px 0;
    height: 80%;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    .textContainerF{
      width: 220px;
      .Text{
        font-size: 15px;
        padding: 10px;
        color: gray;
      }
    }
  }
}

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

.container{
  display: flex;
  justify-content: space-around;
  align-items: center;

}

footer{
  background-image: url(../assets/img//footer-bg.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}

h1{
  text-transform: uppercase;
  font-size: 25px;
}

</style>
