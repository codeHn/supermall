<template>
  <div class="min-tab">
    <router-view/>
    <TabBar>
      <!--      <TabBarItem path="/user" active-color="deep-blue" 控制字体颜色>-->
      <TabBarItem path="/user">
        <!--      <img slot="item-icon" src="~assets/img/user.svg" alt=""> 文件夹别名的使用-->
        <img slot="item-icon" src="assets/img/tabbar/home.svg" alt="">
        <img slot="item-icon-active" src="assets/img/tabbar/home.svg" alt="">
        <div slot="item-text">首页</div>
      </TabBarItem>
      <TabBarItem path="/sub">
        <img slot="item-icon" src="assets/img/tabbar/home.svg" alt="">
        <img slot="item-icon-active" src="assets/img/tabbar/home.svg" alt="">
        <div slot="item-text">通讯录</div>
      </TabBarItem>
      <TabBarItem path="/email">
        <img slot="item-icon" src="assets/img/tabbar/home.svg" alt="">
        <img slot="item-icon-active" src="assets/img/tabbar/home.svg" alt="">
        <div slot="item-text">邮件</div>
      </TabBarItem>
      <TabBarItem path="/setting">
        <img slot="item-icon" src="assets/img/tabbar/home.svg" alt="">
        <img slot="item-icon-active" src="assets/img/tabbar/home.svg" alt="">
        <div slot="item-text">设置</div>
      </TabBarItem>
    </TabBar>
  </div>
</template>

<script>
import TabBar from "./tabbar/TabBar";
import TabBarItem from "./tabbar/TabBarItem";

export default {
  name: "MinTab",
  components: {
    TabBar,
    TabBarItem
  }
}
</script>

<style scoped>
#tab-bar {
  display: flex;
  background-color: #f6f6f6;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  box-shadow: 0 -1px 1px rgba(100, 100, 100, 0.15);
}
</style>