<template>
  <div class="my_nav">
    <div class="nav_box clearfix">
      <div class="log_box fl"></div>
      <a href="javascript:void(0);" class="btn_menu fr" @click="isShow = !isShow"></a>
    </div>
    <ul class="nav_options" v-show="isShow">
      <li class="option" v-for="(route,index) in menuList" :key="index" :class="{'active':routeObj.name === route.name}" @click="jump(route.path)">
        <a href="javascript:void(0);">{{route.menu}}</a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name:'myNav',
  data() {
    return {
      menuList:[
        {name:'index',menu:'首页',path:'/'},
        {name:'Wisdom',menu:'智慧数据',path:'/Wisdom'},
        {name:'About',menu:'关于我们',path:'/About'},
        {name:'Solution',menu:'解决方案',path:'/Solution'}
      ],
      isShow:false
    }
  },
  computed:{
    routeObj(){
      return this.$route
    }
  },
  mounted() {
    console.log(this.routeObj)
  },
  methods:{
    jump(path) {
      this.$router.push({path:path})
      this.isShow = false
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
