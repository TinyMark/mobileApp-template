<template>
  <div id="app">
    <Navbar></Navbar>
    <router-view class="content" />
    <Tabbar></Tabbar>
  </div>
</template>

<style lang="less" scoped>
#app {
  height: 100vh;
  overflow: hidden;
  .content {
    background-color: #eee;
    margin-top: 46px;
    height: calc(100vh - 96px);
    overflow-y: auto;
    font-size: 16px;
    line-height: 1.2;
    padding: 10px;
  }
}
</style>

<script>
import Navbar from '@/components/Navbar'
import Tabbar from '@/components/Tabbar'
export default {
  components: {
    Navbar,
    Tabbar
  }
}
</script>
