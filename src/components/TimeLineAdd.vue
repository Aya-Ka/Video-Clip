<template>
 <v-flex id="time-line-add" offset-xs3 align-self-center>
   <p v-on:click="addTimeLine">+ Tap to add one more timeline</p>
 </v-flex>
</template>


<script>
export default {
  name: "TimeLineAdd",
  methods: {
    addTimeLine() {
      console.log('clicked');
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#time-line-add {
  padding-top: 10px;
  padding-left: 150px;
  padding-right:150px;
}
</style>
