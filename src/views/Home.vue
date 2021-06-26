<template>
  <div class="home">
    <div class="banner">
      <Banner/>
    </div>
  </div>
</template>

<script>
import Banner from '@/components/Banner.vue'
export default {
  name: 'home',
  components: {
    Banner
  }
}
</script>

<style scoped>
.banner {
  height: 100vh;
}
</style>
