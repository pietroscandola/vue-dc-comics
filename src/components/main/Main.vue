<template>
  <main>
    <MainHeader :products='products' />
    <MainFooter />    
  </main>
</template>

<script>
import MainHeader from './MainHeader.vue'
import MainFooter from './MainFooter.vue'

export default {
    name: 'Main',
    components:{
      MainHeader,
      MainFooter,           
    },
    props: ["products"]
}
</script>

<style>

</style>