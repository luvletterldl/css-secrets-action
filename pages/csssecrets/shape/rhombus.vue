<template>
  <div class="container">
    <div class="picture">
      <img src="~/assets/img/rhombus.png" alt="">
    </div>
    <div class="shape">
      <span>这是一个特殊边角的div</span>
    </div>
  </div>
</template>

<style lang="stylus" scoped>
.container
  position absolute
  top 0
  width 100vw
  height 100vh
  .picture
    width 50vw
    height 50vw
    margin 25vw
    overflow hidden
    border pink 1px solid
    transform rotate(45deg)
    img
      /* 这种方式也可以 但是不够优雅
      transform rotate(-45deg)
      max-width 141.4%
      margin -20.7%;
      */
      // transform  rotate(-45deg) scale(1.414) // 使用scale(属性放大)
      // max-width 100%
      // 使用clip-path能最好的解决这种需求 使用时需考虑兼容性问题
      clip-path polygon(50% 0, 100% 50%, 50% 100%, 0 50%)
      transition 1s clip-path
      width 50vw
      height 50vw
    img:hover
      clip-path polygon(0 0, 100% 0, 100% 100%, 0 100%)
  .shape
    height 20vh
    width 80vw
    padding 5vw
    margin 0 10vw
    background lightblue
    // background linear-gradient(-45deg, transparent 15px, lightblue 0)
    background radial-gradient(circle at top left, transparent 15px, #58a 0) top left, radial-gradient(circle at top right, transparent 15px, #58a 0) top right, radial-gradient(circle at bottom right, transparent 15px, #58a 0) bottom right, radial-gradient(circle at bottom left, transparent 15px, #58a 0) bottom left // 弧形切割
    // background linear-gradient(135deg, transparent 15px, #58a 0) top left, linear-gradient(-135deg, transparent 15px, #58a 0) top right, linear-gradient(-45deg, transparent 15px, #58a 0) bottom right, linear-gradient(45deg, transparent 15px, #58a 0) bottom left // 线性切割
    background-repeat no-repeat
    background-size 50% 50%
</style>
