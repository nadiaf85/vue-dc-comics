<template>
  <footer>
    <div class="container">
      <div class="container_bottom">
        <button>SIGN UP NOW!</button>
          <div class="icone">
            <h3>FOLLOW US</h3>
            <img src="../assets/img/footer-facebook.png" alt="">
            <img src="../assets/img/footer-periscope.png" alt="">
            <img src="../assets/img/footer-pinterest.png" alt="">
            <img src="../assets/img/footer-twitter.png" alt="">
            <img src="../assets/img/footer-youtube.png" alt="">
          </div> 
        </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: 'FooterSocial',
    
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

.container_bottom{
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

footer{
  background-color: black;
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  .icone{
    color: $first_color;
    display: flex;
    justify-content: end;
    align-items: center;
  }

  button{
    color: white;
    cursor: pointer;
    background: none;
    border: 1px solid $first_color;
    padding: 10px;
    
    h3{
    color: $first_color;
    }
    img{
      margin: 0 5px;
    }
  }
}

.icone img{
  padding: 8px;
}

  
</style>