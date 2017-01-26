<template>
  <main class="u-cf">
    <side-menu></side-menu>
    <section class="p-main">
      <router-view></router-view>
    </section>
  </main>
</template>

<script>
import TopForm from './TopForm'
import SideMenu from './SideMenu'

export default {
  components: {
    TopForm,
    SideMenu
  }
}
</script>

<style scoped>
main {
  width: 1040px;
  margin: 0 auto;
}
.p-main {
  float: right;
  width: 840px;
  padding-bottom: 120px;
}
</style>