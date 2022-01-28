<template>
  <main>
    <div class="containerMain">
      <div class="immagine_top">
        <Jumbotrone />
      </div>

      <div class="immagine_bottom">
        <div>
          <button class="button_top">current series</button>
        </div>
        <Cards />
      </div>
      <div class="container_bottom">
          <button class="button_bottom">load more</button>
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
@import '../assets/style/partials/variables.scss';
 
main{
  position: relative;
  background-color: black;
}

.immagine_bottom{
  margin-top: 30px;
  height: 508px;
  display: flex;
}

button{
  background-color: $first_color;
  color: white;
  text-transform: uppercase;
  padding: 10px 15px;
  border: none;
}

.button_top{
  top: 304px;
  left: 160px;
  font-size: 18px;
  font-weight: bold;
  position: absolute;
}

.container_bottom{
  display: flex;
}

.button_bottom{
  width: 14%;
  margin: 15px auto;
  height: 43px;
  font-weight: bold;
}


</style>