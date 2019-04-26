<template>
<section>
   <Header/>
   <Footer/>
 </section>
</template>

<script>
import Header from '~/components/Header.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Header,
    Footer

  }
}
function Addmin() {
  alert("sss");
};
</script>

<style lang="sass">
  @import '../assets/variables'
  body
    box-sizing: border-box
    margin: 0 auto
    background: $black-four
</style>
