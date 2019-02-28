<template>
  <section class="page-home">
    <div class="banner_box1">
      <h2 class="tit_cn">海量数据 引领未来</h2>
      <p class="tit_en">Massive Data Leads the Future</p>
      <div class="btn_group">
        <a href="javascript:void(0);" class="wisdom_data">智慧数据</a><a href="javascript:void(0);" class="contact_us">联系我们</a>
      </div>
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
    text-align: center;
    .tit_cn{
      padding-top: 300px;
      font-size: 69px;
      color: #fefeff;
      line-height: 90px;
      
    }
    .tit_en{
      font-size: 36px;
      color: #fefeff;
      line-height: 50px;
    }
    .btn_group{
      padding-top: 58px;
      text-align: center;
      a{
        display: inline-block;
        width: 256px;
        line-height: 80px;
        font-size: 40px;
        color: #ffffff;
        border: 2px solid #ffffff;
      }
      .wisdom_data{
        border-color: #ffcc00;
        color: #ffcc00;
        margin-right: 66px;
      }
    }
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
