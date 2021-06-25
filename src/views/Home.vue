<template>
  <div class="home">
    <Layerout>
      <Header style="height: 100vh">
        <Banner/>
      </Header>
      <Content>
        施工中~
      </Content>
    </Layerout>
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
