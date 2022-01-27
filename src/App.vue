<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from './components/header.vue'
import Main from './components/main.vue'
import Footer from './components/footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer

  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
