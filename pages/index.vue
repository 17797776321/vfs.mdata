<template>
  <section class="page-home">
    <div class="banner_box1">
    </div>
    <div class="banner_box2">
    </div>
    <div class="banner_box3">
    </div>
    <div class="banner_box4">
    </div>
  </section>
</template>

<script>
export default {
  components:{
  },
  name:'Home',
  data() {
    return {}
  }
}
</script>
<style lang="less">
@import '../assets/style/common.less';
.page-home{
  .banner_box1{
    .bgimg(750px,975px,'../images/banner1.png',100%,100%,center,center);
  }
  .banner_box2{
    .bgimg(750px,940px,'../images/banner2.png',100%,100%,center,center);
  }
  .banner_box3{
    .bgimg(750px,1600px,'../images/banner3.png',100%,100%,center,center);
  }
  .banner_box4{
    .bgimg(750px,2658px,'../images/banner4.png',100%,100%,center,center);
  }
}
</style>
