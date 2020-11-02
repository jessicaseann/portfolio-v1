<template>
  <v-app id="app">
    <Navigation/>
    <v-content class="ma-0 pa-0">
      <Portfolio/>
    </v-content>
  </v-app>
</template>

<script>
import Portfolio from './components/Portfolio.vue'
import Navigation from './components/Navigation.vue'

export default {
  name: 'App',
  components: {
    Portfolio,
    Navigation
  },
  data() {
    return {
      options: {
      scrollOverflow: true
    },
  }
}
}
</script>

<style lang='scss'>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap');
$body-page: 'Playfair Display';
.v-application {
  font-family: $body-page !important;
}
body {
  margin: 0 !important;
}
p {
  margin: 0 0 4px 0 !important;
}
</style>
