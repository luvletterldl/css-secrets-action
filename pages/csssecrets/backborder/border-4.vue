<template>
  <div class="con">
    <div class="backborder">
      <div class="back">
        边框内圆角有时我们需要一个容器，只在内侧有圆角，而边框或描边的四个角在外 部仍然保持直角的形状
      </div>
    </div>
    <div class="back-1">
      边框内圆角有时我们需要一个容器，只在内侧有圆角，而边框或描边的四个角在外 部仍然保持直角的形状
    </div>
  </div>
</template>

<style lang="stylus" scoped>
.con
  position absolute
  top 0
  width 100vw
  height 100vh
  background-color #F3F4FE
  .backborder
    background lightskyblue
    height 17vh
    padding 1vh
    margin 3vh 20vw
    .back
      color #ffffff
      font-size small
      height 15vh
      border #58a 1vw solid
      background #58a
      border-radius 1vh
  .back-1
    box-shadow: 0 0 0 0.8vh lightskyblue // box-shadow会跟着元素的圆角走,只要box-shadow的外半径值小于等于outline的值就可以
    outline: 1vh lightskyblue solid // 描边不会跟着元素的圆角走,而是为直角
    width: 57vw
    margin: auto
    color #ffffff
    font-size small
    height 15vh
    border #58a 1vw solid
    background #58a
    border-radius 1vh
</style>
