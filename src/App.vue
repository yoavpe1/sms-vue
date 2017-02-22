<template>
  

  <div id="app">
    <senderInfo></senderInfo>
    <ReceiverInfo></ReceiverInfo>
    <messages></messages>
  </div>
</template>

<script>
import SenderInfo from './components/SenderInfo'
import ReceiverInfo from './components/ReceiverInfo'
import Messages from './components/Messages'

export default {
  name: 'app',
  components: {
    SenderInfo, ReceiverInfo, Messages
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
