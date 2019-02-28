<template>
  <div class="layout">
    <my-nav></my-nav>
    <nuxt class="view_box"/>
    <my-footer></my-footer>
  </div>
</template>
<script>
import myNav from '@/components/myNav'
import myFooter from '@/components/myFooter'
export default {
  name: 'Layout',
  components:{
    myNav,
    myFooter
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
