<template>
<header class="header-bar">

  <nuxt-link onclick="active(event)" to="/" class="header-bar_link active">Главная</nuxt-link>
  <nuxt-link onclick="active(event)" to="/okompanii" class="header-bar_link">О компании</nuxt-link>
  <nuxt-link onclick="active(event)" to="#" class="header-bar_link">Стать субагентом</nuxt-link>
  <nuxt-link onclick="active(event)" to="#" class="header-bar_link">Услуги</nuxt-link>
  <nuxt-link onclick="active(event)" to="#" class="header-bar_link">Контакты</nuxt-link>

   <script type="text/javascript">
    function active(event){
      var target = event.target;
      var i = 0;
      var link = document.getElementsByClassName('header-bar_link');
      link[0].classList.remove('active');
      link[1].classList.remove('active');
      link[2].classList.remove('active');
      link[3].classList.remove('active');
      link[4].classList.remove('active');
      target.classList.add('active');
     }
   </script>

 </header>
</template>

<script>

</script>

<style lang="sass" scoped>
@import '../assets/variables'
.header-bar
  position: relative
  top: 89px
  width: 70%
  display: flex
  height: 28px
  justify-content: space-between
  margin-right: 18%
  &:before
    margin-top: 7px
    content: ""
    display: inline-block
    vertical-align: middle
    width: 42%
    height: 1px
    background: $pinkish-grey
@media screen and (max-width: $adaptive-width)
  .header-bar
    width: 83%
    margin-right: 6%
  .header-bar:before
    width: 47%
.header-bar_link
  font-family: SegoeUI
  font-size: $text-size
  color: $pinkish-grey
  cursor: pointer
  text-decoration: none
  margin-left: 3%
  outline: none
  &:hover
    color: $azure
    border-bottom: 1px solid $azure
    text-decoration: none
  &.active
    color: $azure
    border-bottom: 1px solid $azure
@media screen and (max-width: $adaptive-width)
  .header-bar_link
    margin-left: 40px
    font-size: $adapptive-text
</style>
