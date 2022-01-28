<template>
    <div class="card">
      <div class="containerImg">
        <img :src="details.thumb" alt="">
      </div>
      <h5>{{details.series}}</h5>
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
    margin: 50px 10px 0px 10px;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    .containerImg{
      width: 100%;
      height: 70%;
      overflow: hidden;

      img{
        width: 100%;
      }
    }
  }


</style>