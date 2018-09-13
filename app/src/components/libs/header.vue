<template>
  <div id="header">
    <p v-if="headerType === 1" class="header_p" v-for="(item, index) in headerInfo" :key="index">
      <span class="header_span">{{item.id}}</span>
      <span class="header_span">{{item.id}}</span>
      <span class="header_span">{{item.id}}</span>
      <span class="header_span">{{item.id}}</span>
      <span class="header_span">{{item.id}}</span>
    </p>
    <p v-if="headerType === 2">
      sh
    </p>
  </div>
</template>
<style lang="less" src='@/assets/less/libs/header.less' scoped></style>
<script>
export default{
  name: 'HeaderIndex',
  props: ['headerInfo', 'headerType'],
  /**
   * headerType: num
   * 1.首页头部 左边列表按钮 中间logo 右边购物车
   * 2.返回头部 左边返回按钮 中间页面名称 右边分享按钮
   * 3.搜索头部 左边列表按钮 中间搜索框 右边购物车
   */
  methods: {
    // 返回上一级路由
    back () {
      this.$router.back(-1)
    }
  }
}
</script>
