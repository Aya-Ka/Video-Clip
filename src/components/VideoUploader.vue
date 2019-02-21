<template>
  <div id="uploader">
    <v-layout row>
      <v-flex xs1 offset-xs3>
        <upload-btn 
          title="Upload"
          color="grey lighten-4"
          small
          :fileChangedCallback="fileChanged"
        ></upload-btn>
      </v-flex>
      <v-flex xs4 flex-grow: 0>
        <v-text-field
          height="20px"
          outline
          v-model='filePath'
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
      this.filePath = file.name;
    }
  },
  data: () => ({
    filePath: "Please choose your video file"
  })
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#uploader {
  padding-top: 80px;
  padding-left: 150px;
  padding-right:150px;
}
</style>
