<template>
   <div class="series">
          <img :src="carta.thumb" alt="">
          <h4>{{carta.series}}</h4>
        </div>
</template>

<script>
export default {
    name: 'Card',
    props:{
        carta: Object,
        series: String
    }
}
</script>

<style lang="scss" scoped>
.series{
   width: calc(100% / 6 - 20px);
    margin: 50px 10px 0px 10px;
    flex-direction: row;
    padding: 15px;
    text-align: center;

    img{
    width: 70%;
    height: 150px;
    }
}

h4{
    color: white;
    text-align: center;
}

</style>