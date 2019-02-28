<template>
  <div class="layout">
    <my-nav></my-nav>
    <nuxt class="view_box"/>
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

<style lang="less">
.layout{
  .view_box{
    padding-top: 109px;
  }
}
</style>
