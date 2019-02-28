<template>
  <div class="my_footer">
    <h2 class="tit">联系我们</h2>
    <ul class="options_list">
      <li class="option clearfix" v-for="(item,index) in list" :key="index">
        <div class="img_box fl"><img :src="item.img" alt=""></div>
        <div class="text_box fl">{{item.text}}</div>
      </li>
    </ul>
  </div>
</template>
<script>
import footer1 from '@/assets/images/footer1.png'
import footer2 from '@/assets/images/footer2.png'
import footer3 from '@/assets/images/footer3.png'
import footer4 from '@/assets/images/footer4.png'
export default {
  data() {
    return{
      list:[
        {
          img:footer1,
          text:'郑州市郑东新区绿地之窗景峰座5022'
        },
        {
          img:footer2,
          text:'400-816-7772'
        },
        {
          img:footer3,
          text:'66378@qq.com'
        },
        {
          img:footer4,
          text:'http://www.vfengs.com/'
        },
      ]
    }
  }
}
</script>
<style lang="less">
@import '../../assets/style/common.less';
.my_footer{
  .bgimg(750px,927px,'../images/banner5.png',100%,100%,center,center);
  .tit{
    padding: 68px 30px 25px 30px;
    font-size: 48px;
    font-weight: 500;
    color: #333333;
    line-height: 60px;
    text-align: center;
  }
  .options_list{
    .option{
      padding: 30px 30px 0 30px;
      .img_box{
        width: 136px;
        height: 94px;
        img{
          display: block;
          width: 94px;
          height: 94px;
        }
      }
      .text_box{
        max-width: 505px;
        line-height: 94px;
        padding: 0 25px;
        font-size: 30px;
        color: #6f6e6a;
      }
    }
  }
}
</style>