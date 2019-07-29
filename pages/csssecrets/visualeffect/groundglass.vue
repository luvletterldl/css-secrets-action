<template>
  <div class="container">
    <div class="gglass">
      <span>这是一块毛玻璃特效</span>
      <span>这是一块毛玻璃特效</span>
      <span>这是一块毛玻璃特效</span>
      <span>这是一块毛玻璃特效</span>
    </div>
  </div>
</template>

<style lang="stylus" scoped>
.container
  position absolute
  top 0
  width 100vw
  height 100vh
  background url('../../../assets/img/backage.png') no-repeat
  background-size 100% 100%
  .gglass
    position relative
    background hsla(0,0%,100%,.3)
    overflow hidden
    margin 20vw
    height 40vh
    width 60vw
  .gglass::before
    color #333
    background: url('../../../assets/img/backage.png') 0 / cover fixed;
    content: ''
    position absolute
    top 0
    right 0
    bottom 0
    left 0
    filter blur(20px)
    margin -30px
</style>
