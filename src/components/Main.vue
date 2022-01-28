<template>
  <main>
    <div class="containerMain">
      <div class="immagine_top">
        <immagine-main />
      </div>

      <div class="immagine_bottom">
        <Cards />
      </div>
    </div>
  </main>
</template>

<script>
import ImmagineMain from './commons/ImmagineMain.vue'
import Cards from './sections/Cards.vue'

export default {
    name: 'Main',
    components:{
      ImmagineMain,
      Cards
    }
}
</script>

<style lang="scss" scoped>
 
.immagine_bottom{
  background-color: black;
  margin-top: 30px;
  height: 500px;
  display: flex;
}
</style>