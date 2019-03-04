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
  }
}
</style>
