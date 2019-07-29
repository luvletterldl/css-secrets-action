<template>
  <div class="con">
    <span class="box-shadow">11</span>
    <span class="outline">22</span>
    <span class="outline-1">21</span>
    <span class="shadow">12</span>
    <span class="doubule-shadow">111</span>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="stylus" scoped>
.con
  width 100vw
  height 100vh
  background linear-gradient(#fb3 20%, #58a 80%)
  display flex
  flex-direction column
  align-items center
  justify-content space-evenly
  span
    padding 2vh
  .box-shadow
    background lightskyblue
    box-shadow: 0 0 0vh 1vh lightcyan, 0 0 0vh 2vh lightyellow
  .outline
    background lightyellow
    border 1vh solid lightcyan
    outline 1vh solid lightskyblue
  .outline-1
    background yellowgreen
    border 10px solid #655
    outline 5px solid deeppink
    outline-offset -.5vh
  .shadow
    background #F3FD33
    box-shadow 0 5px 3px -3px #715 // 单侧投影
  .doubule-shadow
    background #F3FD33
    box-shadow 5px 0 5px -5px black, -5px 0 5px -5px black
</style>
