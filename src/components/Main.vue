<template>
  <main>
    <Jumbotron/>
     
  </main>
</template>

<script>
  import Jumbotron from '@/components/Jumbotron.vue'

export default {
  
  name: 'Main',

  components: { 
    Jumbotron 
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

main{
   height: 800px;
} 

h1{
  font-size: 20px;
}
</style>
