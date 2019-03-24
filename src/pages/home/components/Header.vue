<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题</div>
    <div class="header-right">城市
      <span class="iconfont">&#xe64a;</span>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="stylus" scoped>
@import '../../../assets/styles/varibles.styl'
.header
  line-height: 3.583333rem
  background: $bgColor
  display: flex
  color: #ffffff
  .header-left
    width: 2.666667rem
    float: left
    .back-icon
      font-size 1.666667rem
      text-align center
  .header-input
    flex: 1
    background: #ffffff
    border-radius: .416667rem
    height 2.666667rem
    line-height 2.666667rem
    margin-top: .5rem
    margin-left .833333rem
    color #ccc
    padding-left .833333rem
  .header-right
    width: 5.166667rem
    float: right
    text-align: center
</style>
