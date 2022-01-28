<template>
  <main>
    <div class="containerMain">
      <div class="immagine_top">
        <Jumbotrone />
      </div>

      <div class="immagine_bottom">
        <Cards />
      </div>
    </div>
  </main>
</template>

<script>
import Jumbotrone from './commons/Jumbotrone.vue'
import Cards from './sections/Cards.vue'

export default {
    name: 'Main',
    components:{
      Jumbotrone,
      Cards
    }
}
</script>

<style lang="scss" scoped>
 
.immagine_bottom{
  background-color: black;
  margin-top: 30px;
  height: 550px;
  display: flex;
}
</style>