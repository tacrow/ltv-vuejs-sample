<template>
  <div id="app">
    <vue-header></vue-header>
    <vue-main></vue-main>
    <vue-footer></vue-footer>
  </div>
</template>

<script>
import VueHeader from './components/common/Header'
import VueMain from './components/common/Main'
import VueFooter from './components/common/Footer'

export default {
  name: 'app',
  components: {
    VueHeader,
    VueMain,
    VueFooter
  }
}
</script>

<style src="assets/postcss/all.css"></style>
