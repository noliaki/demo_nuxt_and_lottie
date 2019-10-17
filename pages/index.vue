<template>
  <div class="container">
    <Lottie :options="lottieOptions" />
  </div>
</template>

<script>
import Lottie from '~/components/Lottie.vue';
import animationData from '~/assets/SaCSS.json';

export default {
  components: {
    Lottie
  },
  data() {
    return {
      lottieOptions: {
        animationData
      }
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: center / cover no-repeat url("~assets/sapporo.jpg");
  overflow: hidden;
}
</style>
