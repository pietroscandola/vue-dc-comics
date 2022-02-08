<template>
  <main>
    <MainHeader />
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
    }
}
</script>

<style>

</style>