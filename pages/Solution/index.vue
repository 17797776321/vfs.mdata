<template>
  <div class="page-solution">
    <div class="banner_box">
      <h2 class="tit_cn">当数据发出声音时，我们可以帮助您找到最佳倾听方式</h2>
      <p class="tit_en">When data sounds, we can help you find the best way to listen.</p>
    </div>
    <!--能力-->
    <div class="content_box">
      <ul class="ability_box clearfix">
        <li class="option_box fl" v-for="(item,index) in abilityList" :key="index">
          <img :src="item.img" alt="" class="icon">
          <p class="text">{{item.text}}</p>
        </li>
      </ul>
      <div class="pro_box">
        <div class="box" v-for="(item,index) in proList" :key="index">
          <div class="header">{{item.header}}</div>
          <ul class="option_list clearfix">
            <li class="option_box fl" v-for="(nItem,nIndex) in item.options" :key="nIndex">
              <img :src="nItem.img" alt="">
              <h2>{{nItem.tit}}</h2>
              <p>{{nItem.des}}</p>
            </li>
          </ul>
        </div>
      </div>
      <!-- 运营 -->
      <div class="operate_box">
        <div class="header">
          <img src="../../assets/images/operate.png" alt="">
        </div>
        <ul class="list clearfix">
          <li class="industry" :class="{'fl':index%2 === 0,'fr':index%2 === 1}" v-for="(item,index) in industryList" :key="index">
            <img :src="item.img" alt="">
            <div class="content" :class="{'color':item.isColor}">
              <h2 class="tit">{{item.tit}}</h2>
              <p class="des">{{item.des}}</p>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
import ability1 from '@/assets/images/ability1.png'
import ability2 from '@/assets/images/ability2.png'
import ability3 from '@/assets/images/ability3.png'
import ability4 from '@/assets/images/ability4.png'

import prod1 from '@/assets/images/prod1.png'
import prod2 from '@/assets/images/prod2.png'
import prod3 from '@/assets/images/prod3.png'
import prod4 from '@/assets/images/prod4.png'

import industry1 from '@/assets/images/industry1.png'
import industry2 from '@/assets/images/industry2.png'
import industry3 from '@/assets/images/industry3.png'
import industry4 from '@/assets/images/industry4.png'
import industry5 from '@/assets/images/industry5.png'
import industry6 from '@/assets/images/industry6.png'
export default {
  name:'Solution',
  data() {
    return {
      abilityList:[
        {
          img:ability1,
          text:'大数据预测更安全'
        },
        {
          img:ability2,
          text:'大数据预测更安全'
        },
        {
          img:ability3,
          text:'大数据预测更安全'
        },
        {
          img:ability4,
          text:'大数据预测更安全'
        }
      ],
      proList:[
        {
          header:'精准的用户画像能力',
          options:[
            {
              img:prod1,
              tit:'线上行为',
              des:'基于App行为数据'
            },
            {
              img:prod2,
              tit:'线下行为',
              des:'基于场景活动数据'
            }
          ]
        },
        {
          header:'实时的场景捕捉能力',
          options:[
            {
              img:prod3,
              tit:'线上捕捉',
              des:'通过大数据挖掘和行为建模来推测用户当下的手机使用行为场景'
            },
            {
              img:prod4,
              tit:'线下捕捉',
              des:'通过用户线下场景活动数据，分析用户当下时间所处的位置场景'
            }
          ]
        }
      ],
      industryList:[
        {
          img:industry1,
          tit:'移动互联网行业',
          des:'洞察用户属性，提升运营效果，智能解析行业新趋势',
          isColor:false
        },
        {
          img:industry2,
          tit:'金融行业',
          des:'精准客群定位，促进产品推广与转化',
          isColor:true
          
        },
        {
          img:industry3,
          tit:'旅游行业',
          des:'与各省市旅游局合作，监测景区人流状况并智能分析',
          isColor:true
        },
        {
          img:industry4,
          tit:'营销行业',
          des:'通过大数据用户画像与地理位置信息的结合，优化广告投放效果',
          isColor:false
        },
        {
          img:industry5,
          tit:'房地产行业',
          des:'为土地研究、区域规划、房产政策提供数据咨询和指导',
          isColor:false
        },
        {
          img:industry6,
          tit:'公共服务',
          des:'为国家地震灾害、春运等提供数据支持与服务',
          isColor:true
        }
      ]
    }
  }
}
</script>
<style lang="less">
@import '../../assets/style/common.less';
.page-solution{
  .banner_box{
    .bgimg(750px,447px,'../../assets/images/banner_so.png',100%,100%,center,center);
    text-align: center;
    .tit_cn{
      font-size: 25px;
      color: #fefeff;
      line-height: 46px;
      padding-top: 188px;
    }
    .tit_en{
      font-size: 16px;
      color: #fefeff;
      line-height: 26px;
    }
  }
  .content_box{
    background-color: #BBDCF2;
    padding: 30px;
    .ability_box{
      background-color:#FFFFFF;
      .option_box{
        width: 50%;
        text-align: center;
        padding: 44px 0;
        .icon{
          display: block;
          width: 117px;
          margin: 0 auto;
        }
        .text{
          line-height: 20px;
          font-size: 18px;
          color: #666666;
          padding-top: 30px;
        }
      }
    }
    .pro_box{
      .box{
        text-align: center;
        background-color: #E3F4FB;
        margin-top: 30px;
        .header{
          padding-top: 48px;
          font-size: 26px;
          color: #333333;
          line-height: 50px;
        }
        .option_list{
          padding-top: 60px;
          padding-bottom: 55px;
          .option_box{
            width: 50%;
            img{
              display: block;
              width: 100px;
              margin: 0 auto;
            }
            h2{
              line-height: 36px;
              font-size: 22px;
              color: #00a0e9;
              padding-top: 14px;
            }
            p{
              max-width: 290px; 
              font-size: 20px;
              color: #666666;
              line-height: 34px;
              padding-top: 28px;
              margin: 0 auto;
            }
          }
        }
      }
    }
    .operate_box{
      padding: 25px;
      background-color: #E3F4FB;
      margin-top: 30px;
      .header{
        img{
          display: block;
          width: 100%;
        }
      }
      .list{
        margin: 0 auto;
        vertical-align: top;
        .industry{
          width: 310px;
          height: 300px;
          position: relative;
          margin-top: 25px;
          background-color: #ffffff;
          img{
            display: block;
            width: 100px;
            height: 100px;
            position: absolute;
            right: 0;
            bottom: 0;
            z-index: 2;
          }
          .content{
            width: 100%;
            height: 100%;
            position: absolute;
            top: 0;
            left: 0;
            z-index: 3;
            color: #333333;
            .tit{
              padding-top: 34px;
              padding-left: 20px;
              font-size: 28px;
            }
            .des{
              padding: 80px 20px 0 20px;
              font-size: 20px;
            }
          }
          .color{
            background-color: #01ACF3 !important;
            color: #ffffff !important;
          }
        }
      }
    }
  }
}
</style>
