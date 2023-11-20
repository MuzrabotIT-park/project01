<template>
  <body :class="{active: bodyActive}" >
    
    <Navbar @actionBody="bodyActive = true" />
  </body>
</template>

<script>
import Navbar from "./layout/navbar.vue";

export default {
  components: { Navbar },
  data() {
    return {
      bodyActive:false
    }
  },
};
</script>

<style lang="scss">
@import "./assets/styles/main.scss";
body{
  background:$background_color_body ;
  color: $color;

  &.active{
    background: #ffffff !important;
  }
}
</style>
