<template>
  <footer>
    <div class="block">
      <div><img src="/images/logo.png" alt=""></div>
      <span>© 2018 «Авр центр»</span>
    </div>
  </footer>
</template>

<script>
    export default {
        name: "custom-footer",
    }
</script>

<style lang="scss">
  footer {
    background-color: #F8F8F8;
    padding: 30px 4vw;
    .block {
      display: flex;
      flex-direction: column;
      span {
        font-size: 10px;
        color: #888888;
        margin-top: 5px;
      }
    }
  }
</style>
