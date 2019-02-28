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
      <div class="content_box">
        <div class="analysis_box">
          <a href="javascript:void(0);" class="pos1">大数据</a>
          <a href="javascript:void(0);" class="pos2">提高盈利</a>
          <a href="javascript:void(0);" class="pos3">吸引顾客</a>
          <a href="javascript:void(0);" class="pos4">消费数据</a>
          <a href="javascript:void(0);" class="pos5">人工智能</a>
          <h2 class="center_text">智慧数据分析</h2>
        </div>
      </div>
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
    .content_box{
      padding-top: 210px;
      .analysis_box{
        .bgimg(527px,528px,'../images/bcircle.png',100%,100%,center,center);
        margin: 0 auto;
        position: relative;
        text-align: center;
        a{
          display: inline-block;
          .bgimg(107px,107px,'../images/scircle.png',100%,100%,center,center);
          font-size: 20px;
          color:#172027;
          line-height: 107px;
          position: absolute;
        }
        .pos1{
          left: 210px;
          top: -52px;
        }
        .pos2{
          left: -38px;
          top: 130px;
        }
        .pos3{
          left: 455px;
          top: 130px;
        }
        .pos4{
          left: 45px;
          top: 405px;
        }
        .pos5{
          left: 374px;
          top: 405px;
        }
        .center_text{
          font-size: 34px;
          color: #ffffff;
          padding-top: 230px;
        }
      }
    }
  }
  .banner_box3{
    .bgimg(750px,1600px,'../images/banner3.png',100%,100%,center,center);
  }
  .banner_box4{
    .bgimg(750px,2658px,'../images/banner4.png',100%,100%,center,center);
  }
}
</style>
