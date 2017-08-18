<template>
  <div class="hello">
  

  <mt-tab-container v-model="selected">
  <mt-tab-container-item id="tab1">
  <mt-header fixed title="联系人"></mt-header>
  <!-- 搜索框 -->
  <mt-search></mt-search>
  <!-- tab标签 -->
<mt-navbar v-model="select">
  <mt-tab-item id="tab-container1">我的好友</mt-tab-item>
  <mt-tab-item id="tab-container2">陌生人</mt-tab-item>
  <mt-tab-item id="tab-container3">黑名单</mt-tab-item>
</mt-navbar>

<!--联系人内容-->
  <mt-tab-container v-model="select">
  <mt-tab-container-item id="tab-container1">  
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >陈奕迅</span><img slot="icon" src="../assets/cyx.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >薛之谦</span><img slot="icon" src="../assets/xzq.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >陈冠希</span><img slot="icon" src="../assets/cgx.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >周柏豪</span><img slot="icon" src="../assets/zbh.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >陈伟霆</span><img slot="icon" src="../assets/cwt.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >马云</span><img slot="icon" src="../assets/my.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >迪丽热巴</span><img slot="icon" src="../assets/dlrb.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >奥特曼</span><img slot="icon" src="../assets/atm.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >谢腾飞</span><img slot="icon" src="../assets/xtf.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >宋民国</span><img slot="icon" src="../assets/smg.jpg" width="45px" height="45px"></mt-cell>
  </mt-tab-container-item>
  <mt-tab-container-item id="tab-container2">
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >小丸子</span><img slot="icon" src="../assets/people.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >哆啦A梦</span><img slot="icon" src="../assets/people.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >吴若楠</span><img slot="icon" src="../assets/people.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >美少女</span><img slot="icon" src="../assets/people.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >卡布达</span><img slot="icon" src="../assets/people.jpg" width="45px" height="45px"></mt-cell>
    <mt-cell title=""><span style="margin:10px -310px 5px -310px;color:black" >迪迦</span><img slot="icon" src="../assets/people.jpg" width="45px" height="45px"></mt-cell>
  </mt-tab-container-item>
  <mt-tab-container-item id="tab-container3">
    <mt-cell v-for="n in 5" title=""><span style="margin:10px -310px 5px -310px;color:black" >手机用户148958</span><img slot="icon" src="../assets/people.jpg" width="45px" height="45px"></mt-cell>
  </mt-tab-container-item>
</mt-tab-container>

  <!-- <mt-search v-model="value"> -->

<!-- </mt-search> -->
  </mt-tab-container-item>
  <mt-tab-container-item id="tab2">
  <mt-header fixed title="消息">
  <router-link to="/" slot="left">
    <mt-button icon="back">back</mt-button>
  </router-link>
  </mt-header>
  <!-- 搜索框 -->
  <mt-search></mt-search>
  <mt-cell style="text-align:left;">
  <img slot="icon" src="../assets/my.jpg" width="45px" height="45px">
  <span style="margin:10px 200px 5px 0px;color:black" >马云</span>
  <span>人呢？</span>
  <mt-badge size="small" color="red">10</mt-badge>
  </mt-cell>
  <mt-cell style="text-align:left;">
  <img slot="icon" src="../assets/xzq.jpg" width="45px" height="45px">
  <span style="margin:10px 209px 5px 0px;color:black" >薛之谦</span>
  <span>小傻瓜</span>
  <!-- <mt-badge size="small" color="red">5</mt-badge> -->
  </mt-cell>
  <mt-cell style="text-align:left;">
  <img slot="icon" src="../assets/zbh.jpg" width="45px" height="45px">
  <span style="margin:10px 95px 5px 0px;color:black" >周柏豪</span>
  <span>几时落课，我去接你</span>
  <mt-badge size="small" color="red">2</mt-badge>
  </mt-cell>
  <mt-cell style="text-align:left;">
  <img slot="icon" src="../assets/cgx.jpg" width="45px" height="45px">
  <span style="margin:10px 158px 5px 0px;color:black" >陈冠希</span>
  <span>一齐食饭？</span>
  <mt-badge size="small" color="red">3</mt-badge>
  </mt-cell>
  <mt-cell style="text-align:left;">
  <img slot="icon" src="../assets/dlrb.jpg" width="45px" height="45px">
  <span style="margin:10px 105px 5px 0px;color:black" >迪丽热巴</span>
  <span>记得看我的新电影~</span>
  </mt-cell>
  <mt-cell style="text-align:left;">
  <img slot="icon" src="../assets/xtf.jpg" width="45px" height="45px">
  <span style="margin:10px 145px 5px 0px;color:black" >谢腾飞</span>
  <span>小姐姐带我去玩</span>
  </mt-cell>
  <mt-cell style="text-align:left;">
  <img slot="icon" src="../assets/smg.jpg" width="45px" height="45px">
  <span style="margin:10px 190px 5px 0px;color:black" >宋民国</span>
  <span>사랑해</span>
  <mt-badge size="small" color="red">9</mt-badge>
  </mt-cell>
  <mt-cell style="text-align:left;">
  <img slot="icon" src="../assets/people.jpg" width="45px" height="45px">
  <span style="margin:10px 60px 5px 0px;color:black" >【陌生人】小丸子</span>
  <span>hi~加个好友呗</span>
  <mt-badge size="small" color="orange">...</mt-badge>
  </mt-cell>
  </mt-tab-container-item>
  <mt-tab-container-item id="tab3">
  <mt-header fixed title="搜索">
  <router-link to="/" slot="left">
    <mt-button icon="back">back</mt-button>
  </router-link>
  </mt-header> 
  <mt-search></mt-search>
    <mt-cell to="http://news.qq.com/a/20170818/029711.htm" title="[国际] 西班牙恐袭事件推升全球金融市场避险情绪"></mt-cell>
    <mt-cell to="http://news.qq.com/a/20170818/027959.htm" title="[国际] 外媒：巴塞罗那恐怖袭击第3名嫌疑人被捕"></mt-cell>
    <mt-cell to="http://news.qq.com/a/20170818/028795.htm" title="[国内] 5年来对口支援西藏及四省藏区工作回顾"></mt-cell>
    <mt-cell to="http://news.qq.com/a/20170818/025386.htm" title="[国内] 北京等9城房价下跌 专家预计楼市最高峰已过去"></mt-cell>
    <mt-cell to="http://news.qq.com/a/20170818/025277.htm" title="[社会] 男子吃过期10年飞机餐"></mt-cell>
    <mt-cell to="http://news.qq.com/a/20170818/019346.htm" title="[社会] 男子报警称儿子被绑架 原是丢条狗怕警方不重视"></mt-cell>
	<mt-cell to="http://news.qq.com/a/20170818/027689.htm#p=1" title="[图片] 洪水冲毁15年植树成果 残疾哥俩重头再来"></mt-cell>
	<mt-cell to="http://news.qq.com/a/20170818/025353.htm#p=1" title="[图片] 【图话】对“坏蜀黍”说不！"></mt-cell>

  </mt-tab-container-item>
  <mt-tab-container-item id="tab4">
  <mt-header fixed title="我的">
  <router-link to="/" slot="left">
    <mt-button icon="back">back</mt-button>
  </router-link>
  </mt-header>

<mt-cell value="用户名：Coco"is-link>
<img slot="icon" src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1503030976924&di=c74afc8721ad68ea7c4b5454a2952acf&imgtype=0&src=http%3A%2F%2Fimg16.3lian.com%2Fgif2016%2Fq23%2F69%2F81.jpg" width="100px" height="100px">
</mt-cell>
<mt-cell title="新消息通知" style="text-align:left;">
<mt-switch v-model="value"></mt-switch>
  <span></span>
</mt-cell>
<mt-cell title="账号与安全" is-link  style="text-align:left;">
  <span></span>
</mt-cell>
<mt-cell title="帮助与反馈" is-link  style="text-align:left;">
  <span></span>
</mt-cell>
<mt-cell title="我的相册" is-link  style="text-align:left;">
  <span></span>
</mt-cell>
<mt-cell title="系统设置" is-link  style="text-align:left;">
  <span></span>
</mt-cell>
<mt-button type="primary" style="width:360px;margin-bottom:10px">切换账号</mt-button><br/>
<mt-button type="danger"  style="width:360px">退出登录</mt-button>
  </mt-tab-container-item>
</mt-tab-container>

  <mt-tabbar v-model="selected">
  <mt-tab-item id="tab1">
  <i class="fa fa-group fa-lg"></i><br/><br/>
    <!-- <img slot="icon" src="../assets/100x100.png"> -->
    联系人
  </mt-tab-item>
  <mt-tab-item id="tab2">
  <i class="fa fa-envelope fa-lg"></i><br/><br/>
    <!-- <img slot="icon" src="../assets/100x100.png"> -->
    消息
  </mt-tab-item>
  <mt-tab-item id="tab3">
  <i class="fa fa-search fa-lg"></i><br/><br/>
    <!-- <img slot="icon" src="../assets/100x100.png"> -->
    搜索
  </mt-tab-item>
  <mt-tab-item id="tab4">
  <i class="fa fa-user-circle-o fa-lg"></i><br/><br/>
    <!-- <img slot="icon" src="../assets/100x100.png"> -->
    我的
  </mt-tab-item>
</mt-tabbar>
  </div>
</template>

<script>
import { Header } from 'mint-ui';
export default {
  name: 'hello',
  data () {

    return {
    	selected:'tab1',
    	select:'tab-container1',
    	msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>
	.mint-search {height: 50px;}
	.mint-cell img {float: left;}
	.mint-cell{padding:-2px 10px;text-align:left;line-height: -150px;}
	html{margin:-20px -10px ; }
</style>