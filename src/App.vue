<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
import AppBlueLine from './components/AppBlueLine.vue'
export default {
  components: {
    AppHeader,
    AppMain,
    AppBlueLine,
    AppFooter
  }
}
</script>
<template>
  <AppHeader />
  <AppMain />
  <AppBlueLine />
  <AppFooter />
</template>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  background-color: rgb(36, 36, 36);
}
</style>