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
      <div class="header">我们能做什么</div>
      <ul class="main_box">
        <li class="option" v-for="(item,index) in projectList" :key="index">
          <div class="top_box clearfix">
            <div class="icon_box fl">
              <img :src="item.img" alt="">
            </div>
            <div class="title fl">{{item.tit}}</div>
          </div>
          <div class="content_box">
            {{item.des}}
          </div>
        </li>  
      </ul>
    </div>
    <div class="banner_box4">
      <h2 class="header">我们的优势</h2>
      <div class="main">
        <ul class="card_list">
          <li class="card_box" v-for="(item,index) in cardList" :key="index" :class="{'mt':index !== 0}">
            <div class="top_box">
              <div class="img_box">
                <img :src="item.img" alt="">
              </div>
              <h2 class="tit">{{item.tit}}</h2>
            </div>
            <div class="content_box">
              <p class="des">{{item.des}}</p>
              <p class="option" v-for="(nItem,nIndex) in item.options" :key="nIndex">{{nItem}}</p>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
import pro1 from '@/assets/images/pro1.png'
import pro2 from '@/assets/images/pro2.png'
import pro3 from '@/assets/images/pro3.png'
import pro4 from '@/assets/images/pro4.png'

import card1 from '@/assets/images/card1.png'
import card2 from '@/assets/images/card2.png'
import card3 from '@/assets/images/card3.png'
export default {
  components:{
  },
  name:'Home',
  data() {
    return {
      projectList:[
        {
          img:pro1,
          tit:'营销云',
          des:'全媒体整合多渠道广告触达,线上线下数据搜集实现场景化营销,唯一恪守贴牌定制合作模式,自主溢价模式利润高。'
        },
        {
          img:pro2,
          tit:'数据管理DMP',
          des:'全媒体整合多渠道广告触达,释放数据价值，提升营销效果全面精确的人群管理安全、开放、专业。'
        },
        {
          img:pro3,
          tit:'智子盒子',
          des:'人工智能营销管家，线上线下数据汇通融合，智慧零售零距离营销，打破线下实体营销困境。'
        },
        {
          img:pro4,
          tit:'大数据解决方案',
          des:'广告转化预测模型和系统解决方案，广告投放CTR预测模型解决方案，数据标签化处理和资产变现解决方案，个性化推荐解决方案。'
        }
      ],
      cardList:[
        {
          img:card1,
          tit:'数据管理',
          des:'基于云计算，为企业提供数据收集、抓取、集成、处理等定制化服务，制定一体化数据管理解决方案',
          options:['大数据云平台的搭建','数据集成','数据采集']
        },
        {
          img:card2,
          tit:'数据分析',
          des:'深入理解企业业务逻辑，为企业提供定制化的数据收集、清洗、建模、分析、可视化等服务。',
          options:['数据建模服务','算法支撑服务','数据可视化服务']
        },
        {
          img:card3,
          tit:'系统定制开发',
          des:'完善企业业务流程系统，建立销售平台、客户关系管理、风险防范等互联网弹性架构，实现多维度后台实时查询和监测。',
          options:['CRM系统','金融业务系统']
        }
      ]
    }
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
    .bgimg(690px,1540px,'../images/banner3.png',100%,100%,center,center);
    padding: 30px;
    .header{
      font-size: 48px;
      color: #cb0000;
      text-align: center;
    }
    .main_box{
      .option{
        padding-top: 36px;
        .top_box{
          .icon_box{
            width: 129px;
            img{
              display: block;
              width: 100%;
            }
          }
          .title{
            font-size: 45px;
            color:#172027;
            line-height: 129px;
            padding-left: 20px;
          }
        }
        .content_box{
          padding-top: 25px;
          font-size: 28px;
          color: #172027;
          line-height: 44px;
        }
      }
    }
  }
  .banner_box4{
    .bgimg(750px,2658px,'../images/banner4.png',100%,100%,center,center);
    .header{
      padding: 67px 0;
      font-size: 48px;
      color: #333333;
      line-height: 74px;
      text-align: center;
    }
    .main{
      .card_list{
        .mt{
          margin-top: 66px !important;
        }
        .card_box{
          width: 554px;
          height: 696px;
          margin: 0 auto;
          border: 2px #E4E4E4 solid;
          background-color: #ffffff;
          .top_box{
            background-color: #4E95FF;
            .img_box{
              padding-top: 44px;
              img{
                display: block;
                width: 122px;
                margin: 0 auto;
              }
            }
            .tit{
              font-size: 32px;
              color: #ffffff;
              text-align: center;
              padding-top: 30px;
              line-height: 66px;
            }
          }
          .content_box{
            padding: 30px;
            .des{
              line-height: 40px;
              font-size: 25px;
              color: #9d9d9d;
              text-align: center;
              padding: 10px 0 30px 0;
            }
            .option{
              text-align: center;
              font-size: 25px;
              color: #333333;
              line-height: 56px;
              font-weight: 600px;
            }
          }
        }
      }
    }
  }
}
</style>
