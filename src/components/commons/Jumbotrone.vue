<template>
<div class="containerMain">
  <div class="hero">
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
  height: 290px;
}

.hero{
  height: 320px;
  width: 100%;
  background-image: url(../../assets/img/jumbotron.jpg) ;
  background-position: top;
  background-repeat: no-repeat;
  background-size: cover;
}

</style>