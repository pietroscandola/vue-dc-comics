<template>
  <div class="container">
    <Header/>
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
   Header,
  }
}
</script>

<style lang="scss">
.container{
  max-width: 1200px;
  margin: 0 auto;
}
</style>
