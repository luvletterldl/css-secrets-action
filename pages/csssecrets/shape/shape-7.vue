<template>
  <div class="con">
    <div class="oval" />
    <div class="rhomboid">伪元素实现字体不倾斜</div>
  </div>
</template>

<style lang="stylus" scoped>
.con
  position absolute
  display: flex
  flex-direction: column
  justify-content: center
  align-items: center
  top 0
  .oval
    background #95e
    height 25vw
    width 25vh
    margin 10vw
    // border-radius 20px 10px 30px 40px / 50px 20px 40px 25px
    // border-top-right-radius 20px
    border-radius 50% / 100% 100% 0 0
    // border-radius 100% 0 0 100% / 50%
    border-radius 100% 0 0 0 // 1/4椭圆
  .rhomboid
    color #ffffff
    position: relative
  .rhomboid::before
    content: ''; /* 用伪元素来生成一个矩形 */
    position: absolute;
    top: 0; right: -3vw; bottom: 0; left: -3vw
    z-index: -1;
    background: #d69;
    transform: skew(45deg);
</style>
