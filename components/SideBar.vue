<template>
 <div class="sidebar">
   <nuxt-link class="side-bar_main" to="#">Войти&nbsp;&nbsp;&nbsp;&#8594;</nuxt-link>
   <nuxt-link class="side-bar_link" to="#">Авиабилеты</nuxt-link>
   <nuxt-link class="side-bar_link" to="#">Ж/Д билеты</nuxt-link>
   <nuxt-link class="side-bar_link" to="#">Гостиницы</nuxt-link>
   <nuxt-link class="side-bar_link" to="#">Страхование</nuxt-link>
   <nuxt-link class="side-bar_link" to="#">Трансфер</nuxt-link>
 </div>
</template>

<script>

</script>

<style lang="sass" scoped>
@import '../assets/variables'
.sidebar
  display: flex
  position: relative
  font-family: SegoeUI
  background: $black-two
  width: 12%
  min-width: 175px
  font-size: 12px
  height: 1272px
  flex-direction: column
  border-left: 1px solid $pinkish-grey
  padding-left: 45px
@media screen and (max-width: $adaptive-width)
  .sidebar
    font-size: $adapptive-text
    padding-left: 3%
.side-bar_link
  position: relative
  top: 200px
  color: $pinkish-grey
  display: flex
  text-decoration: none
  margin:
    top: 76px
.side-bar_main
  position: relative
  top: 93px
  color: $azure
  text-decoration: none

.side-bar_link:before
  position: absolute
  top: 52px
  width: 10px
  border-top: 1px solid $pinkish-grey
  content: ""
.side-bar_link:nth-child(6):before
  border: none
</style>
