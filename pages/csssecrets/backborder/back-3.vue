<template>
  <div class="con">
    <div class="back" />
  </div>
</template>

<style lang="stylus" scoped>
.con
  position absolute
  top 0
  width 100vw
  height 100vh
  background-color #F3F4FE
  .back
    height 30vh
    margin 3vh
    border #58a 1vw solid
    background url(https://cdn2.didiapp.com/continuous/7vip.png) no-repeat bottom right #58a
    background-position: top calc(100% - 30px) left calc(100% - 40px)
    background-origin content-box // 默认情况下，background-position 是以 padding box 为准的 background-position 属 性中使用的边角关键字将会以内容区的边缘作为基准(也就是说，此时背景 图片距离边角的偏移量就跟内边距保持一致了)
    background-size 30% 30%
    img
      width 20vw
      height 20vw
</style>
