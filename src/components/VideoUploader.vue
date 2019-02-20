<template>
  <div id="uploader">
    <v-layout row wrap>
      <v-flex xs1 class="text-xs-center">
        <upload-btn 
          title="Upload"
          color="grey lighten-4"
          small
          :fileChangedCallback="fileChanged"
        ></upload-btn>
      </v-flex>
      <v-flex xs9 offset-xs2 flex-grow: 0>
        <v-text-field
          single-line
          outline
          height="5px"
        ></v-text-field>
      </v-flex>
    </v-layout>
  </div>
</template>

<script>
import UploadButton from 'vuetify-upload-button';

export default {
  name: "VideoUploader",
  components: {
    'upload-btn': UploadButton
  },
  methods: {
    fileChanged(file) {
      console.log(file);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#uploader {
  padding-top: 80px;
  padding-left: 150px;
  padding-right:150px;
  /*background-color: red;*/
}
#styled-input {
  height: 80px;
  font-size: 20pt;
}
</style>
