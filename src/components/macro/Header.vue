<template>
  <div>
    <header>
      <div class="container">
        <div class="headerLeft">
          <div id="logo">
            <img src="../../assets/img/dc-logo.png" alt="">
          </div>
        </div>

        <div class="headerRight">
          <nav>
            <ul>
              <li v-for="(element, index) in links" :key="index">
                <a href="#" :class='{active: element.current==true}'>{{element.text}}</a>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data (){
    return{
      links:[
        {
          text: "characters",
          url:"#",
          current: false,
        },
        {
          text: "comics",
          url:"#",
          current: true,
        },
        {
          text: "movies",
          url:"#",
          current: false,
        },
        {
          text: "Tv",
          url:"#",
          current: false,
        },
        {
          text: "games",
          url:"#",
          current: false,
        },
        {
          text: "collectibles",
          url:"#",
          current: false,
        },
        {
          text: "videos",
          url:"#",
          current: false,
        },
        {
          text: "fans",
          url:"#",
          current: false,
        },
        {
          text: "news",
          url:"#",
          current: false,
        },
        {
          text: "shop",
          url:"#",
          current: false,
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
  justify-content: space-between;
  align-items: center;
}
.headerLeft{
  height: 60px;
  #logo{
    height: 100%;
    img{
      height: 100%;

    }
  }
}
.headerRight{
  width: 650px;
  nav{
    line-height: 80px;
    ul{
      display: flex;
      justify-content: space-between;
      list-style-type: none;
      li{
        a{
          color: black;
          font-size: 13px;
          font-weight: 800;
          text-decoration: none;
          padding-bottom: 30px;
          text-transform: uppercase;
          &:hover{
            border-bottom:4px solid $colorBlue;
            color: $colorBlue;
          }
        }
      }
    }
  }
}

.active{
  color: $colorBlue !important;
  border-bottom:4px solid $colorBlue;
}



</style>
