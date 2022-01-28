<template>
  <footer>
    <div class="barra_blu">   
      <div class="container">
        <div class="container_icone" v-for="(element,index) in icons" :key="index">
           <img :src="element.image" alt="">
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
                image: require("../assets/img/buy-comics-digital-comics.png")
            },
            {
                text: "DC Merchandise",
                image: require("../assets/img/buy-comics-merchandise.png")
            },
            {
                text: "Subscription",
                image: require("../assets/img/buy-comics-subscriptions.png")
            },
            {
                text: "Comic shop locator",
                image: require("../assets/img/buy-comics-shop-locator.png")
            },
            {
                text: "Dc power visa",
                image: require("../assets/img/buy-dc-power-visa.svg")
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
    height: 150px;
    display: flex;
    padding: 15px 20px;
    text-transform: uppercase;
}

.container_icone{
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