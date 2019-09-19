<template>
  <div>
    <!-- 上栏标题 -->
    <div class="header">
      <div class="header-left">
        <div class="iconfont back-icon">&#xe65b;</div>
      </div>
      <div class="title">
        <span>去哪儿攻略</span>
      </div>
      <div class="myTravel">
        <img class="my-icon" src="">
        <span class="my-icon-title">我的游记</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TestHeader'
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.header{
    display: flex;
    justify-content : space-between;
    line-height: $headerHight;
    background: $bgColor;
    color: #fff;
  }
</style>
