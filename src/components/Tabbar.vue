<template>
  <van-tabbar route v-model="active">
    <van-tabbar-item to="/home" name="home" icon="home-o">主页</van-tabbar-item>
    <van-tabbar-item to="/search" name="search" icon="search">搜索</van-tabbar-item>
    <van-tabbar-item to="/friends" name="friends" icon="friends-o">个人中心</van-tabbar-item>
    <van-tabbar-item to="/setting" name="setting" icon="setting-o">设置</van-tabbar-item>
  </van-tabbar>
</template>

<script>
import { Tabbar, TabbarItem } from 'vant'
export default {
  components: {
    vanTabbar: Tabbar,
    vanTabbarItem: TabbarItem
  },
  data () {
    return {
      active: 'home'
    }
  }
}
</script>

<style>
</style>
