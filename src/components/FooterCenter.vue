<template>
  <div>
    <footer>
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
              <h1>shop</h1>
              <div class="Text">
                <div>Shop DC</div>
                <div>Shop DC Collectibles</div>
              </div>
            </div>
             <div class="textContainerF">
              <h1>DC</h1>
              <div class="Text">
                <div>Terms Of Use</div>
                <div>Privacy policy (New)</div>
                <div>Ad Choices</div>
                <div>Advertising</div>
                <div>Jobs</div>
                <div>Subscriptions</div>
                <div>Taleent</div>
                <div>CPSC Certificates</div>
                <div>Rating</div>
                <div>Shop Help</div>
                <div>Contact Us</div>
              </div>
              
            </div>
             <div class="textContainerF">
              <h1>sites</h1>
              <div class="Text">
                <div>DC</div>
                <div>MAD Magazine</div>
                <div>DC Kids</div>
                <div>DC Universe</div>
                <div>DC Powwer Visa</div>
              </div>
              
            </div>
            
          
            

          </div>
          
        </div>
      </div>
    </footer>   
  </div>
</template>

<script>


export default {
  name: 'FooterCenter',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.container{
  display: flex;
  justify-content: space-around;
  align-items: center;

}

.footerCenter{
  height: 500px;
  width: 100%;
  background-image:url(../assets/img/dc-logo-bg.png);
  background-position: right;
  background-repeat: no-repeat;
  .containerTextFooterC{
    margin: 60px 0;
    width: 400px;
    height: 77%;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    .textContainerF{
      width: 175px;
      .Text{
        font-size: 15px;
        padding: 20px 0;
        color: gray;
        div{
          padding: 2px 0;
        }
      }
    }
  }
}



h1{
  text-transform: uppercase;
  font-size: 25px;
}

</style>
