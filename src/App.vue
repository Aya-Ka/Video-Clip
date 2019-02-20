<template>
  <v-app>
    <v-content>
      <Header/>
      <Panel/>
    </v-content>
  </v-app>
</template>

<script>
import Header from './components/Header'
import Panel from './components/Panel'

export default {
  name: 'App',
  components: {
    Header,
    Panel
  },
  data () {
    return {
      //
    }
  }
}
</script>
