<template>
  <div id="app">
    <!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
        <test/>
<!--    <webrtc rtsp="rtsp://wowzaec2demo.streamlock.net/vod/mp4:BigBuckBunny_115k.mp4"/>-->
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import webrtc from './components/webrtc/'
import test from './components/test.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    webrtc,
    test
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
