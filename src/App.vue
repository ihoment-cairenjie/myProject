<template>
  <div id="nav">
    <Test></Test>
  </div>
</template>

<script>
import {
  onMounted,
  onBeforeMount

} from 'vue'
import Test from '@/components/Test'
export default {
  name: 'App',
  components: {
    Test
  },
  setup (props, ctx){

    onMounted(()=>{
      console.log('onMounted')
    })

    onBeforeMount(()=>{
      console.log('onBeforeMount')
    })

    console.log('setups')
  }
}
</script>

<style lang="scss">

</style>
