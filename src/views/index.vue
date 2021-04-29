<template>
  <div class="bodys">
    <van-nav-bar>
        <template  #left>
            <img src="../../public/img/logo.png" alt="">
        </template>
      <template #right>
        <van-icon name="user-o" color="#999999"><br>
            <span>
                我的
            </span>
        </van-icon>
        <van-icon name="wap-nav" color="#999999"><br>
            <span>
            导航
        </span>
        </van-icon>
      </template>
    </van-nav-bar>
    <van-row gutter="20">
  <van-col span="8"><span class="a">户型</span>   <van-icon name="arrow-down" /></van-col>
  <van-col span="8"><span class="a">区域</span><van-icon name="arrow-down" /></van-col>
  <van-col span="8"><span class="a">分格 </span> <van-icon name="arrow-down" /></van-col>
</van-row>
    <van-grid :gutter="10" :column-num="2">
  <van-grid-item v-for="value in 18" :key="value" icon="photo-o" text="文字" >
      <van-image
  width="100%"
  height="100%"
  src="https://img01.yzcdn.cn/vant/cat.jpeg"
/>
<span>
    <b>澳美文化的抽象美感</b>
</span>
<p>
    <span>混搭</span>
    <span>三室</span>
    <span>1100/m</span>
</p>
  </van-grid-item>
</van-grid>
    <div class="tab">
        <div class="tab1">
            <b class="b">上一页</b>
        </div>
        <div class="tab2">
            <b class="b1">2/30</b>
        </div>
        <div class="tab3">
            <b class="b">下一页</b>
        </div>
    </div>
    <div class="c">
    <p class="p" style="text-indent:2em;">
        房先生互联网公司有别于传统装修公司与其他装修中<br>
        介平台，以自莹模式整合设计师与项目经理，杜绝项目转<br>
        包外包，利用互联网将工地在线全景直播，通过去中间环<br>
        提供装修套餐+个性化定制服务。
    </p>
    </div>
    <div class="x">
        <div class="x1">
            <p>
                <span  class="f">
                <van-icon name="phone-o" />
                    服务热线：400-997-658
                </span>
            </p>
        </div>
        <div class="x2">
            <van-row type="flex" justify="space-between">
                <van-col span="6">触摸版</van-col>
                <van-col span="6">电脑版</van-col>
                <van-col span="6">关于我们</van-col>
                <van-col span="6">联系我们</van-col>
        </van-row>
        </div>
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            
        }
    },
};
</script>

<style scoped>
.f{
    font-size: 14px;
    margin-left: 80px;
    /* position: relative; */
    top: 10px;
}
.x{
    width: 94%;
    margin-left: 10px;
    height: 120px;
    background-color: #fff
}
.x1{
    width: 100%;
    height: 60px;
    /* background-color: rosybrown; */
}
.x2{
    width: 100%;
    height: 60px;
    /* background-color: skyblue; */
}
.p{
    font-size: 14px;
}
span{
    font-size: 10px;
    margin-left: 2px;
    margin-left: 5px;
}
img{
    height: 90%;
}
.a{
    font-size: 15px;
    margin-left: 24px;
}
van-grid{
    margin-top: 15px;
}
.bodys{
    background-color: #eaeaea;
}
van-col{
    background-color: #fff;
}
.tab{
    height: 50px;
    width: 94%;
    background-color: red;
    margin-left: 10px;
    margin-top: 15px;
    display: flex;
}
.tab1{
    width: 40%;
    height: 50px;
    background-color: #39c894;
}
.tab2{
    width: 35%;
    height: 50px;
    background-color: #fff;
}
.tab3{
    width: 40%;
    height: 50px;
    background-color: #39c894;
}
.b{
    margin-left: 30px;
    position: relative;
    top: 14px;
}
.b1{
    margin-left: 30px;
    position: relative;
    top: 14px;
    font-size: 18px;
}
.c{
    width: 94%;
    height: 100px;
    margin-left: 10px;
    background-color: #fff;
    margin-top: 10px;
}
</style>