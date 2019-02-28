<template>
  <div>
    <my-nav></my-nav>
    <nuxt />
  </div>
</template>
<script>
import myNav from '@/components/myNav'
export default {
  name: 'Layout',
  components:{
    myNav
  }
}
</script>

<style>
</style>
