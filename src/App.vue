<template>
  <div>
    <Header/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/main/Main.vue'
import Footer from './components/footer/Footer.vue'

export default {
  name: 'App',
  components: {
   Header,
   Main,
   Footer,
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
  margin:20px 0;
  background-color: black;
}

.container{
  max-width: 1200px;
  margin: 0 auto;
}
</style>
