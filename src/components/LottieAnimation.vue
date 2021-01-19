<template>
  <div ref="loadingLottie"></div>
</template>

<script>
import lottie from 'lottie-web';

export default {
  name: 'Loading',
  props: {
    data: Object,
    lottie: Object,
  },
  mounted() {
    this.lottie = lottie.loadAnimation({
      container: this.$refs.loadingLottie,
      renderer: 'svg',
      loop: true,
      autoplay: true,
      animationData: this.data,
    });
  },
  destroy() {
    this.lottie?.destroy();
  }
}
</script>
