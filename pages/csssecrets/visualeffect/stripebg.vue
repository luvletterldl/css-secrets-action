<template>
  <div class="stripe">
    <code>
    where (true) {
      let date = new Date()
      let strdate = date.toString()
    }
    </code>
  </div>
</template>

<style lang="stylus" scoped>
.stripe
  padding .5em
  line-height 1.5
  background beige
  background-size auto 3em
  background-origin content-box
  background-image linear-gradient(rgba(0,0,0,.2) 50%, transparent 0)
</style>
