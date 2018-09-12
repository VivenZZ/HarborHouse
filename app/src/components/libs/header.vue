<template>
  <div id="header">
    <p class="header_p" v-for="(item, index) in headerInfo" :key="index">
      <span class="header_span">{{item.id}}</span>
    </p>
  </div>
</template>
<style lang="less" src='@/assets/less/libs/header.less' scoped></style>
<script>
export default{
  name: 'HeaderIndex',
  props: ['headerInfo']
}
</script>
