<template>
    <div class="card">
      <div class="containerImg">
        <img :src="details.thumb" alt="">
      </div>
      <div class="containerText">
        <h5>{{details.series}}</h5>
      </div>
    </div> 
</template>

<script>
export default {
  name: 'SeriesCardsContainer',
  props: {
    details: Object,
  }

}
</script>

<style lang="scss" scoped>
  .card{
    width: calc(100% / 6 - 20px);
    margin: 20px 10px;
    height: 200px;
    
   
    
    .containerImg{
      width: 100%;
      height: 170px;
      overflow: hidden;

      img{
        width: 100%;
      }
    }
    h5{
      height: 20px;
      padding: 5px 0;
    }
    .containerText{
      height: 30px;
    }
  }



</style>