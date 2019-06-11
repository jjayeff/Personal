<template>
  <app-home/>
</template>

<script>
  import appHome from './components/home';

  export default {
    components: {
      appHome
    }
  }
</script>

<style lang="scss">
  * {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  html {
    background: #fff;
    color: #333;
    font-family: 'Lato', sans-serif;
  }

  .container {
    max-width: 1140px;
    margin: 0 auto;
  }
  
</style>
