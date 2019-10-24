<template>
  <div class="row mt-4">
    <div class="col-md-7">
      <vue-dropzone
        class="my-4"
        ref="myVueDropzone"
        id="dropzone"
        :options="dropzoneOptions"
        :useCustomSlot=true
        @vdropzone-complete="afterComplete"
      >
        <div class="dropzone-custom-content">
          <h3 class="dropzone-custom-title">Drag and drop to upload content!</h3>
          <div class="subtitle">...or click to select a file from your computer</div>
        </div>
      </vue-dropzone>
    </div>
    <div class="col-md-5 text-right my-5">
      <button class="btn btn-success btn-lg compress-button">
        Compress
      </button>
    </div>
  </div>
</template>

<script>
import vue2Dropzone from 'vue2-dropzone'
import 'vue2-dropzone/dist/vue2Dropzone.min.css'

export default {
  data () {
    return {
      dropzoneOptions: {
        url: 'https://httpbin.org/post',
        thumbnailWidth: 150,
        maxFilesize: 4,
        maxFiles: 1,
        acceptedFiles: '.jpeg, .jpg, .png, .svg',
        // headers: { 'My-Awesome-Header': 'header value' },
        addRemoveLinks: true
      }
    }
  },
  methods: {
    afterComplete (files) {
      console.log(files)
    }
  },
  components: {
    vueDropzone: vue2Dropzone
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
$primary-color:  #00b782;
$secondary-color: #fff;

#dropzone {
  border-radius: 5px;
  border-style: dashed;
  border-color: $primary-color;
}
.dropzone-custom-content {
  position: relative;
  top: 27px;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

.dropzone-custom-title {
  margin-top: 0;
  color: $primary-color;
}

.subtitle {
  color: $primary-color;
}
.compress-button {
  background-color: $primary-color;
  border-color: $primary-color;
  padding: 0.3rem 3rem;
}
</style>
