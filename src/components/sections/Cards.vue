<template>
  <section>
    <div class="container_cards">
        <!-- <div class="series">
          <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
          <h4>nome</h4>
        </div> -->
        <Card v-for="(element,index) in carte" :key="index" :carta="element" :series="element.series"/>
        <SeriesData/>
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

.container_cards{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}


</style>