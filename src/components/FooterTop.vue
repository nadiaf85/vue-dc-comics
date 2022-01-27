<template>
  <footer>
    <div class="barra_blu">   
      <div class="container">
        <div class="container_icons" v-for="(element,index) in icons" :key="index">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <p>{{element.text}}</p>
        </div>
      </div>
  </div>
  </footer>
</template>

<script>
export default {
    name: 'FooterTop',
    data() {
      return{
        icons: [
            {
                text: "Digital comics",
            },
            {
                text: "DC Merchandise",
            },
            {
                text: "Subscription",
            },
            {
                text: "Comic shop locator",
            },
            {
                text: "Dc power visa",
            },
        ]
      }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

.container{
  display: flex;
  justify-content: space-around;
}

.barra_blu{
    background-color: $first_color;
    height: 200px;
    display: flex;
    padding: 15px 20px;
    text-transform: uppercase;
}

.container_icons{
  display: flex;
  align-items: center;
  font-size: 13px;
  
  img{
    width: 50px;
    height: 60px;
    margin-right: 10px;
  }
  p{
    color: white;
    text-transform: uppercase;
  }
}

</style>