<template>
   <div id="panel">
     <VideoUploader/>
     <TimeInput/>
     <VideoSourceAdd/>
     <Run/>
   </div>
 </template>
 
<script>
import VideoUploader from './VideoUploader'
import TimeInput from './TimeInput'
import VideoSourceAdd from './VideoSourceAdd'
import Run from './Run'

export default {
  name: 'Panel',
  components: {
    VideoUploader,
    TimeInput,
    VideoSourceAdd,
    Run
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#panel {
  height: calc(100% - 160px);
  width: calc(100% - 80px);
  background-color: white;
  margin-top: -20px;
  margin-left: 40px;
  margin-right: 40px;
  margin-bottom: 10px
}

</style>
