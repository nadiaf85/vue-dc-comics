<template>
  <section>
      <div class="container">
        <div class="container_cards">
            <Card v-for="(element,index) in carte" :key="index" :carta="element" :series="element.series"/>
            <seriesData/>
        </div>
    </div>
  </section>

</template>

<script>
import Card from '../commons/Card.vue'
import seriesData from '../../data/series.js'


export default {
    name: 'Cards',
    components: {
        Card,
        seriesData
    },
    data (){
        return {
            carte: seriesData
            }
    }
}
</script>

<style lang="scss" scoped>

section{
    width: 100%;
}

.container_cards{
    width: 1100px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;

}


</style>