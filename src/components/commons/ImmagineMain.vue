<template>
<div class="containerMain">
  <div class="hero">
    <img src="../../assets/img/jumbotron.jpg" alt="">
  </div>
</div>
</template>

<script>
export default {
    name: 'ImmagineMain'
}
</script>

<style lang='scss' scoped>

.containerMain{
  width: 100%;
  height: 300px;
}

.hero{
  img{
  width: 100%;
  height: 400px;
  background-repeat: no-repeat;
  background-size: cover;
  }
}

</style>