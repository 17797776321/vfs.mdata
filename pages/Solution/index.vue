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
    </div>
  </div>
</template>
<script>
import ability1 from '@/assets/images/ability1.png'
import ability2 from '@/assets/images/ability2.png'
import ability3 from '@/assets/images/ability3.png'
import ability4 from '@/assets/images/ability4.png'
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
  }
}
</style>
