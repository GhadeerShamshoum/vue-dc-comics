<template>
  <main>
    <Jumbotron/>
    <div class="container">
      <button class="button-top">current series</button>
    </div>
    <div class="container">
    <SeriesCardsContainer
    v-for="(element, index) in series"
    :key="index"
    :details="element"/>
    </div>
    <div class="container">
      <button class="button-bottom">load more</button>
    </div>
     
  </main>
</template>

<script>
  import Jumbotron from '../commons/Jumbotron.vue'
  import SeriesCardsContainer from '../commons/SeriesCardsContainer.vue'
  import seriesdata from '../../data/Series.js'
  
export default {
  
  name: 'Main',

  components: { 
    Jumbotron,
    SeriesCardsContainer 
  },

  data() {
    return {
      series: seriesdata
    }
    
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../../assets/style/partials/variables.scss';

main{
   height: 958px;
   position: relative;
} 

h1{
  font-size: 20px;
}

.container{
    margin: 20px auto;
    width: 1100px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

button{
  background-color: $colorBlue;
  color: white;
  text-transform: uppercase;
  padding: 10px 15px;
  border: none;
}

.button-top{
  font-size: 20px;
  font-weight: 700;
  position: absolute;
  top:296px;
  left: 198px; 
}

.button-bottom{
  width: 180px;
  margin-top: 35px;
}


</style>
