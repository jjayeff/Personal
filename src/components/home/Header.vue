<template>
  <header>
    <app-navbar :data='narbar'/>
    <app-video-header/>
  </header>
</template>

<script>
import appNavbar from '../core/Navbar1.vue';
import appVideoHeader from './components/VideoHeader.vue';
export default {
  components: {
    appNavbar,
    appVideoHeader
  },
  data() {
    return {
      narbar: {
        logo: 'ekkawit',
        lists: [
          'about me',
          'portfolio',
          'experience',
          'contact',
        ],
      }
    }
  }
}

</script>

<style lang="scss" scoped>
  header {
    position: relative;
    width: 100%;
    height: 100vh;
    overflow: hidden;
    background: rgba(0, 0, 0, 0.7);
  }
</style>
