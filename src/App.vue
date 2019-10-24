<template>
  <div id="app">
    <app-header></app-header>
    <div class="container">
      <app-dropzone></app-dropzone>
    </div>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Dropzone from './components/Dropzone'
import Header from './components/layout/header.vue'
import Footer from './components/layout/footer.vue'

export default {
  name: 'app',
  components: {
    appDropzone: Dropzone,
    appHeader: Header,
    appFooter: Footer
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  color: #2c3e50;
  background-color: #F3F4F5;
}
</style>
