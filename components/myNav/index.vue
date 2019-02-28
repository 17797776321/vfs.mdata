<template>
  <div class="my_nav">
    <div class="nav_box clearfix">
      <div class="log_box fl"></div>
      <a href="javascript:void(0);" class="btn_menu fr" @click="isShow = !isShow"></a>
    </div>
    <ul class="nav_options" v-show="isShow">
      <li class="option active">
        <a href="javascript:void(0);">首页</a>
      </li>
      <li class="option">
        <a href="javascript:void(0);">智慧数据</a>
      </li>
      <li class="option">
        <a href="javascript:void(0);">解决方案</a>
      </li>
      <li class="option">
        <a href="javascript:void(0);">关于我们</a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name:'myNav',
  data() {
    return {
      isShow:false
    }
  }
}
</script>
<style lang="less">
@import '../../assets/style/common.less';
.my_nav{
  position: fixed;
  top: 0;
  z-index: 999;
  .nav_box{
    width: 690px;
    padding: 30px;
    background: #232425;
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
  .nav_options{
    background-color: #ffffff;
    box-shadow: 0 0 10px rgba(0,0,0,0.15);
    .option{
      padding: 20px;
      line-height: 44px;
      a{
        display: block;
        font-size: 26px;
        color: #333333;
      }
    }
    .active{
      background-color: #f7f7f7;
    }
  }
}
</style>
