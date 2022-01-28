<template>
  <footer>
    <footer-head />
    <footer-main />
    <footer-lower />
  </footer>
</template>

<script>
import FooterHead from './sub-components/footer-head.vue'
import FooterLower from './sub-components/footer-lower.vue'
import FooterMain from './sub-components/footer-main.vue'
export default {
  components: { 
    FooterHead,
    FooterMain,
    FooterLower 
  },

  name:'Footer'
}
</script>

<style lang="scss" scoped>



</style>