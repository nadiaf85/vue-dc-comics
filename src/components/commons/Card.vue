<template>
   <div class="series">
       <div class="container-carte">
           <img :src="carta.thumb" alt="">
       </div>
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

.container-carte{
    width: 100%;
    height: 155px;
    overflow: hidden;
}

.series{
    width: calc(100% / 6 - 20px);
    margin: 50px 10px 0px 10px;
    flex-direction: row;
    text-align: center;

    img{
    width: 100%;
    }
}

h4{
    font-size: 12px;
    color: white;
    text-transform: uppercase;
    margin-top: 20px;
    font-weight: 200;
    text-align: initial;
}

</style>