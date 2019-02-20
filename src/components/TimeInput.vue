<template>
 <div id="time-input">
   <v-layout row wrap>
     <v-flex xs1 offset-xs3>
     <p>Clip From</p>
     </v-flex>
     <v-flex><v-text-field
        single-line
        outline
      ></v-text-field></v-flex>
     <v-flex><p>To</p></v-flex>
     <v-flex><v-text-field
        single-line
        outline
      ></v-text-field></v-flex>
  </v-layout>
  <TimeLineAdd/>
 </div>
</template>


<script>
import TimeLineAdd from "./TimeLineAdd"

export default {
  name: "TimeInput",
  components: {
    TimeLineAdd
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#time-input {
  padding-top: 20px;
  padding-left:150px;
  padding-right:150px;
  /*background-color:blue;*/
}
</style>
