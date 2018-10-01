<template>
  <div id="app">
    <lcrg-header>Header</lcrg-header>
    <hr/>
  <div id="server-info">
    <servers></servers>
    <server-details></server-details>
  </div>
  <hr/>
  <lcrg-footer></lcrg-footer>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
import Servers from './components/Servers.vue'
import ServerDetails from './components/ServerDetails.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    'lcrg-header': Header,
    Servers,
    ServerDetails,
    'lcrg-footer': Footer
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 20px;
}
#server-info {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
