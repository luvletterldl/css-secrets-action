<template>
  <div class="con" />
</template>

<style lang="stylus" scoped>
.con
  position absolute
  top 0
  width 100vw
  height 100vh
  // background linear-gradient(#fb3 20%, #58a 80%) // 从上20%到下80%处过渡

  // background linear-gradient(#fb3 50%, #58a 50%) // 非平滑过渡

  // background linear-gradient(#fb3 50%, #58a 0%) // 非平滑过渡 + 条纹 如果我们把第二个色标的位置值设置为 0，那它的位置就 总是会被浏览器调整为前一个色标的位置值，这个结果正是我们想要的。
  // background-size 100% 30%

  // background: linear-gradient(#fb3 33.3%, #58a 0, #58a 66.6%, yellowgreen 0) // 三条纹
  // background-size: 100% 45px

  // background linear-gradient(to right, #fb3 50%, #58a 0) // 垂直条纹
  // background-size 5vw 100%

  // background linear-gradient(45deg, #fb3 25%, #58a 0, #58a 50%, #fb3 0, #fb3 75%, #58a 0)
  // background-size 28.28vw 28.28vw

  // background repeating-linear-gradient(45deg, #fb3, #58a 30px)

  background repeating-linear-gradient(60deg, #fb3, #fb3 5vw, #58a 0, #58a 10vw)
</style>
