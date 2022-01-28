<template>
  <header>
      <div class="container">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="">
            
        </div>

        <nav>
          <ul>
            <li v-for="(element, index) in links" :key="index">
              <a href="#" :class="{'active': element.current==true}">{{element.text}}</a>
            </li>
          </ul>
        </nav>
      </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return{
        links: [
            {
                text: "Characters",
                url: "#",
                current: false,
            },
            {
                text: "Comics",
                url: "#",
                current: true,
            },
            {
                text: "Movies",
                url: "#",
                current: false,
            },
            {
                text: "TV",
                url: "#",
                current: false,
            },
            {
                text: "Games",
                url: "#",
                current: false,
            },
            {
                text: "Collectibles",
                url: "#",
                current: false,
            },
            {
                text: "Videos",
                url: "#",
                current: false,
            },
            {
                text: "Fans",
                url: "#",
                current: false,
            },
            {
                text: "News",
                url: "#",
                current: false,
            },
            {
                text: "Shop",
                url: "#",
                current: false,
            },
        ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  @import '../assets/style/partials/variables.scss';

.container{
  display: flex;
  justify-content: space-between;
  align-items: center;
}
  .logo{
    display: flex;
    width: 25%;
    padding: 8px;
  }

  nav{

    ul{
    list-style-type: none;
    display: flex;
    justify-content: center;
    }

    li a{
      display: inline-block;
      color: #000;
      padding: 15px 20px;
      text-decoration: none;
      text-transform: uppercase;
      font-size: 13px;
      font-weight: 800;

      &:hover{
        border-bottom:4px solid $first_color;
        color: $first_color;
      }
    }
  }

  .active{
        border-bottom:4px solid $first_color;
        color: $first_color;
  }
</style>
