<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe65b;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe661;</span>
      输入城市/景点/游玩主题
    </div>
    <router-link to="/city">
      <div class="header-right">
        {{this.city}}
        <span class="iconfont arrow-icon">&#xe6a2;</span>
      </div>
    </router-link>
  </div>
</template>

<script>
import { mapState } from 'vuex'
export default {
  name: 'HomeHeader',
  computed: {
    ...mapState(['city'])
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header{
    display: flex;
    line-height: $headerHight;
    background: $bgColor;
    color: #fff;
  }
    .header-left{
      width:.64rem;
      float:left;
    }
      .back-icon{
        text-align: center;
        font-size: .4rem;
      }
    .header-input{
      flex: 1;
      height: .64rem;
      line-height: .64rem;
      border-radius: .1rem;
      margin-top: .12rem;
      margin-left: .2rem;
      border-right: .1rem;
      padding-left: .2rem;
      background: #fff;
      color: #ccc;
    }
    .header-right{
      min-width: 1.04rem;
      padding: 0 .1rem;
      float: right;
      text-align: center;
      color: #fff;
    }
      .arrow-icon{
        font-size: .24rem;
      }
</style>
