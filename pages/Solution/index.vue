<template>
  <div class="page-solution">
    <div class="banner_box">
      <h2 class="tit_cn">当数据发出声音时，我们可以帮助您找到最佳倾听方式</h2>
      <p class="tit_en">When data sounds, we can help you find the best way to listen.</p>
    </div>
  </div>
</template>
<script>
export default {
  name:'Solution',
  data() {
    return {}
  }
}
</script>
<style lang="less">
@import '../../assets/style/common.less';
.page-solution{
  .banner_box{
   .bgimg(750px,447px,'../../assets/images/banner_so.png',100%,100%,center,center);
    .tit_cn{}
    .tit_en{}
  }
}
</style>
