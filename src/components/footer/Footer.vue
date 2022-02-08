<template>
  <div>
      <TopFooter />
      <BottomFooter />
  </div>
</template>

<script>
import TopFooter from "./TopFooter.vue"
import BottomFooter from "./BottomFooter.vue"
export default {
    name:'Footer',
    components:{
        TopFooter,
        BottomFooter,
    }

}
</script>

<style>

</style>