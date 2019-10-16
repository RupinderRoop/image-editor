<template>
  <div id="app">
    <div class="container">
      <app-header></app-header>
      <app-dropzone></app-dropzone>
    </div>
  </div>
</template>

<script>
import Dropzone from './components/Dropzone'
import Header from './components/layout/header.vue'

export default {
  name: 'app',
  components: {
    appDropzone: Dropzone,
    appHeader: Header
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
