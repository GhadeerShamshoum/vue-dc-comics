<template>
  <main>
    <Jumbotron/>
    <div class="container">
    <SeriesCardsContainer
    v-for="(element, index) in series"
    :key="index"
    :details="element"/>
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

main{
   height: 1000px;
} 

h1{
  font-size: 20px;
}

.container{
    margin: 0 auto;
    width: 1100px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}


</style>
