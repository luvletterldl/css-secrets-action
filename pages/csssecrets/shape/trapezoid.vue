<template>
  <div class="contianer">
    <span class="trapezoid">我是一个梯形</span>
  </div>
</template>

<style lang="stylus" scoped>
.contianer
  position absolute
  top 0
  width 100vw
  .trapezoid
    position relative
    display inline-block
    margin 10vw
    padding .5em 1em .35em
    color white
  .trapezoid::before
    transform rotateX(45deg)
    content '' /* 用伪元素来生成一个矩形 */
    position absolute
    top 0
    right 0
    bottom 0
    left 0
    z-index -1
    background #58a
    transform perspective(.5em) rotateX(5deg)
</style>
