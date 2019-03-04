<template>
  <div class="page-about">
    <div class="banner1_box">
      <h2>我们一直在路上</h2>
    </div>
    <div class="banner2_box"></div>
    <div class="content_box">
      <h2 class="title">河南微风尚科技有限公司</h2>
      <div class="text_box">
        <p class="content_text">河南微风尚科技是一家专业的大数据分析服务公司，大数据分析行业开拓者，为客户提供深度用户行为分析平台、以及专业的咨询服务和行业解决方案，致力于帮助客户实现数据驱动。通过用户精准分群、灵活创建并管理营销活动计划，一键执行计划触达用户，并实时分析活动效果，真正形成自动化、精细化的运营闭环。小微数据立足大数据及用户行为分析的技术与实践前沿，业务现已覆盖以互联网、金融、零售快消、高科技、旅游等为代表的十多个主要行业、并可支持企业多个职能部门。</p>
        <p class="content_text">我们的客户来自各行各业，为了共同目标，我们在工作上密切配合，从创业型小企业到知名品牌，感谢他们对我们的高要求从不同领域给我们带来的挑战，让我们激情的团队有机会用头脑与智慧不断的给客户带来惊喜。</p>
        <p class="content_text">在我国大数据基础建设蓬勃发展的时代，小微数据将更积极、创新地加入企业基础数据源建设、互联网+创新业务发展、大数据技术的深化应用，与各行业领先企业一起构建可持续竞争力，为客户带来价值、重构中国互联网数据根基。</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'About',
  data() {} 
}
</script>
<style lang="less">
@import '../../assets/style/common.less';
.page-about{
  .banner1_box{
    .bgimg(750px,447px,'../../assets/images/about1.png',100%,100%,center,center);
    h2{
      padding-top: 188px;
      font-size: 52px;
      color: #fefeff;
      line-height: 70px;
      text-align: center;
      letter-spacing: 25px;
    }
  }
  .banner2_box{
    margin-top: 22px;
    .bgimg(750px,200px,'../../assets/images/about2.png',100%,100%,center,center);
  }
  .content_box{
    padding: 25px 35px;
    .title{
      font-size: 26px;
      color: #0f78e6;
      line-height: 34px;
      padding-bottom: 15px;
      position: relative;
      &::after{
        content: "";
        display: block;
        width: 40px;
        height: 4px;
        background-color: #006FE4;
        position:absolute;
        bottom: 0px;
        left: 2px;
      }
    }
    .text_box{
      padding-top: 12px;
      .content_text{
        font-size: 22px;
        color: #83868f;
        line-height: 34px;
        text-indent: 30px;
      }
    }
  }
}
</style>
