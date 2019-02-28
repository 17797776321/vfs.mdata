<template>
  <div class="my_nav">
    <div class="nav_box clearfix">
      <div class="log_box fl"></div>
      <a href="javascript:void(0);" class="btn_menu fr"></a>
    </div>
    <ul class="nav_options">
      <li></li>
    </ul>
  </div>
</template>
<script>
export default {
  name:'myNav',
  data() {
    return {}
  }
}
</script>
<style lang="less">
@import '../../assets/style/common.less';
.my_nav{
  width: 690px;
  padding: 30px;
  background: #232425;
  position: fixed;
  top: 0;
  .nav_box{
    .log_box{
      vertical-align: top;
      .bgimg(172px,48px,'../../assets/images/logo.png',100%,100%,center,center)
    }
    .btn_menu{
      vertical-align: top;
      padding-right: 30px;
      .bgimg(47px,47px,'../../assets/images/menu.png',47px,47px,left,center)
    }
  }
}
</style>
