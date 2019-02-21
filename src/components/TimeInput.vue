<template>
 <div id="time-input">
   <v-layout row>
     <v-flex xs1 offset-xs4 align-self-center>
     <p>Clip From</p>
     </v-flex>
     <v-flex xs1><v-text-field
        single-line
        outline
        height=20px
      ></v-text-field></v-flex>
     <v-flex xs1 align-self-center><p>To</p></v-flex>
     <v-flex xs1><v-text-field
        single-line
        outline
        height=20px
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
}
</style>
