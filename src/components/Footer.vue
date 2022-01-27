<template>
  <div>
    <FooterTop/>
    <FooterSottomenu/>
    <FooterSocial/>
  </div>
</template>

<script>
import FooterTop from "./FooterTop.vue";
import FooterSottomenu from "./FooterSottomenu.vue";
import FooterSocial from "./FooterSocial.vue";
export default {
  name: 'Footer',
  components: {
    FooterTop,
    FooterSottomenu,
    FooterSocial
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>