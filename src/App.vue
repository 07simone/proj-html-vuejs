<template>
  <div id="app">
    
    <IndexHeader />
    <IndexMain />
    <IndexJumbotron />
    <IndexThumbnails />
    <IndexContact />
  </div>
</template>

<script>

import IndexHeader from './components/IndexHeader.vue'
import IndexMain from './components/IndexMain.vue'
import IndexJumbotron from './components/IndexJumbotron.vue'
import IndexThumbnails from './components/IndexThumbnails.vue'
import IndexContact from './components/IndexContact.vue'
export default {
  name: 'App',
  components: {
    IndexHeader,
    IndexMain,
    IndexJumbotron,
    IndexThumbnails,
    IndexContact
  }
}
</script>

<style lang="scss">
@import"@/style/main-style.scss";
</style>
