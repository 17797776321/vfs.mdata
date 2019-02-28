<template>
  <div class="page-wisdom">
    <div class="banner1_box"></div>
    <div class="banner2_box"></div>
    <div class="banner3_box"></div>
    <div class="banner4_box"></div>
    <div class="banner5_box"></div>
    <div class="banner6_box"></div>
  </div>
</template>
<script>
export default {
  name: 'Wisdom',
  data() {
    return{}
  },
  mounted() {
  }
}
</script>
<style lang="less">
@import '../../assets/style/common.less';
.page-wisdom{
  .banner1_box{
    .bgimg(750px,447px,'../images/wisdom1.png',100%,100%,center,center);
  }
  .banner2_box{
    .bgimg(750px,247px,'../images/wisdom2.png',100%,100%,center,center);
  }
  .banner3_box{
    .bgimg(750px,273px,'../images/wisdom3.png',100%,100%,center,center);
  }
  .banner4_box{
    .bgimg(750px,274px,'../images/wisdom4.png',100%,100%,center,center);
  }
  .banner5_box{
    .bgimg(750px,274px,'../images/wisdom5.png',100%,100%,center,center);
  }
  .banner6_box{
    .bgimg(750px,275px,'../images/wisdom6.png',100%,100%,center,center);
  }
}
</style>
