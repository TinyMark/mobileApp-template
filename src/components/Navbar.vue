<template>
  <van-nav-bar
    fixed
    :title="title"
    :left-arrow="showLeftArrow"
    :left-text="leftText"
    :right-text="rightText"
    @click-left="onClickLeft"
    @click-right="onClickRight"
  />
</template>

<script>
import { NavBar } from 'vant'
export default {
  props: {
    showLeftArrow: {
      type: Boolean,
      default: () => true
    },
    title: {
      type: String,
      default: () => 'title'
    },
    leftText: {
      type: String,
      default: () => ''
    },
    rightText: {
      type: String,
      default: () => ''
    }
  },
  components: {
    vanNavBar: NavBar
  },
  methods: {
    onClickLeft () {
      this.$router.go(-1)
    },
    onClickRight () {}
  }
}
</script>

<style>
</style>
