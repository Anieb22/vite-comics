<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
import AppBlueLine from './components/AppBlueLine.vue'
import AppJumbotron from './components/AppJumbotron.vue'
export default {
  components: {
    AppHeader,
    AppJumbotron,
    AppMain,
    AppBlueLine,
    AppFooter
  }
}
</script>
<template>
  <AppHeader />
  <AppJumbotron />
  <AppMain />
  <AppBlueLine />
  <AppFooter />
</template>

<style lang="scss">
@use "src/style/generals.scss" as *;
@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200;300;400;500;600;700&display=swap');
</style>