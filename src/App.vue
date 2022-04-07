<template>
  <div id="app">
    
    <IndexMain />
    <Indexjumbotron />
  </div>
</template>

<script>

import IndexMain from './components/IndexMain.vue'
import Indexjumbotron from './components/Indexjumbotron.vue'
export default {
  name: 'App',
  components: {
    IndexMain,
    Indexjumbotron
  }
}
</script>

<style lang="scss">
@import"@/style/main-style.scss";
</style>
