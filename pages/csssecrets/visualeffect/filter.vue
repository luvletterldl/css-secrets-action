<template>
  <div class="container">
    <div class="filter-one">
      <img class="filter" src="~/assets/img/filter.jpg" alt="">
      <img class="unfilter" src="~/assets/img/filter.jpg" alt="">
    </div>
  </div>
</template>

<style lang="stylus" scoped>
.container
  position absolute
  top 0
  width 0
  .filter-one
    width 80vw
    padding 10vw
    .filter
      width 80vw
      filter sepia(0.05) saturate(1.5) hue-rotate(15deg)
    .unfilter
      transition .5s filter
      filter sepia(0.05) saturate(1.5) hue-rotate(15deg)
      width 80vw
    .unfilter:hover, .unfilter:focus
      width 80vw
      filter none
</style>
