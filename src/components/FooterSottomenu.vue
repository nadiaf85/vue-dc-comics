<template>
  <footer>
    <div class="container">
      <div class="sottomenu_lista">
        <ul v-for="(element, index) in categorie" :key="index">{{element.text}}
          <li v-for="(element, index) in categorie[index].content" :key="index">{{element.text}}</li>
        </ul>
        <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'FooterSottomenu',
    data() {
    return{
      categorie:[
          {
          text: "DC Comics",
          content:[
            {
              text: "Characters"
            },
            {
              text: "Comics"
            },
            {
              text: "Movies"
            },
            {
              text: "TV"
            },
            {
              text: "Games"
            },
            {
              text: "Videos"
            },
            {
              text: "News"
            },
          ]
          },
          {
          text: "Shop",
          content:[
            {
              text: "Shop DC"
            },
            {
              text: "Shop DC Collectibles"
            },
          ]
          },
          {
          text: "DC",
          content:[
            {
              text: "Term of Use"
            },
            {
              text: "Privacy Policy (New)"
            },
            {
              text: "Ad Choiches"
            },
            {
              text: "Advertising"
            },
            {
              text: "Jobs"
            },
            {
              text: "Subscriptions"
            },
            {
              text: "Talent Workshops"
            },
            {
              text: "CPSC Certificates"
            },
            {
              text: "Ratings"
            },
            {
              text: "Shop Help"
            },
            {
              text: "Contact Us"
            },
          ]
          },
          {
          text: "Sites",
          content:[
            {
              text: "DC"
            },
            {
              text: "MAD Magazine"
            },
            {
              text: "DC Kids"
            },
            {
              text: "DC Universe"
            },
            {
              text: "DC Power Visa"
            },
          ]
          },
      ]
    }
  }
    
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

footer{
  width: 100%;
  height: 400px;
  background-image: url("../assets/img/footer-bg.jpg");
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;

.sottomenu_lista{
  display: flex;
  margin-top: 30px;
  justify-content: space-around;

  img{
    width: 28%;
  }

  ul{
    width: 100px;
    color: white;
    list-style: none;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 16px;
    margin-bottom: 15px;

    li{
      color: white;
      text-transform: capitalize;
      font-size: 11px;
      margin: 10px 0;
      }
    }
  }
}
  
</style>