<template>
  <div>
    <navbar/>
    <div class="content">
      <nuxt/>
    </div>
  </div>
</template>

<script>
  import Navbar from '~/components/Navbar.vue'
  import Modal from "../components/Modal";

  export default {
    components: {
      Modal,
      Navbar
    }
  }
</script>

<style lang="scss">
  html {
    font-family: "Roboto-Light";
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }

  *, *:before, *:after {
    box-sizing: border-box;
    margin: 0;
  }

  @font-face {
    font-family: 'Roboto-Regular';
    src: url('../static/fonts/Roboto/Roboto-Regular.ttf') format('truetype');
  }
  @font-face {
    font-family: 'Roboto-Light';
    src: url('../static/fonts/Roboto/Roboto-Light.ttf') format('truetype');
  }

  @import "../assets/scss/main";


</style>
