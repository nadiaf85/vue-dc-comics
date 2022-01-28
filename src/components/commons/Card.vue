<template>
   <div class="series">
          <img :src="carta.src" :alt="carta.series">
          <h4>{{carta.thumb}}</h4>
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
    width: calc(25% - 4px);
    margin: 2px;
    padding: 15px;
}

h4{
    color: white;
    text-align: center;
}

</style>