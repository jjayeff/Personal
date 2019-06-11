<template>
  <div class="test">
    <video class="video-container" autoplay loop muted>
      <source src="../../../assets/video/Fast Typing - 1656.mp4" type="video/mp4">
    </video>
    <div class="welcome-msg">
      <h1>my name is Ekkawit</h1>
      <app-type-text-effect class="text-animation"/>
    </div>
  </div>
</template>

<script>
  import appTypeTextEffect from '../../core/TypeTextEffect.vue';
  export default {
    components: {
      appTypeTextEffect
    }
  }
</script>

<style lang="scss">
  .video-container {
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    z-index: -1;
  }
  @media (min-aspect-ratio:16/9) {
    .video-container {
      width: 100%;
      height: auto;
    }
  }
  @media (max-aspect-ratio:16/9) {
    .video-container {
      width: auto;
      height: 100%;
    }
  }
  .welcome-msg {
    position: absolute;

    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    h1 {
      text-align: center;
      margin-top: 0;
      margin-bottom: 20px;
      color: #fff;
      font-size: 240%;
      text-transform: uppercase;
      letter-spacing: 10px;
      word-spacing: 4px;

      animation: moveInLeft 1s ease-out;
    }

    .text-animation {
      animation: moveInRight 1s ease-out;
    }

    .btn-center {
      position: absolute;
      left: 50%;
      transform: translate(-50%);
    }
  }

  @keyframes moveInLeft {
    0% {
      opacity: 0;
      transform: translateX(-10rem);
    }

    80% {
      transform: translateX(1rem)
    }

    100% {
      opacity: 1;
      transform: translate(0);

    }
  }
  @keyframes moveInRight {
    0% {
      opacity: 0;
      transform: translateX(1rem);
    }

    80% {
      transform: translateX(-1rem)
    }

    100% {
      opacity: 1;
      transform: translate(0);

    }
  }


</style>

