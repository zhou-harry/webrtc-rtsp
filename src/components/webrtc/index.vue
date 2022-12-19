<template>
  <div>
    <h2>webrtc-vue测试</h2>
    <video id="video" style="width: 100%;height: 100%;"/>
  </div>
</template>

<script>
import WebRtcStreamer from './webrtcstreamer.js'

export default {
  props: {
    server: {
      type: String,
      default: 'http://10.41.88.99:8000'
    },
    rtsp: String
  },
  data() {
    return {
      webRtcServer: {}
    }
  },
  mounted() {
    console.log("打开连接==============")
    let options = "rtptransport=tcp";
    this.webRtcServer = new WebRtcStreamer("video", this.server);
    this.webRtcServer.connect(this.rtsp, null, options);
  },
  beforeDestroy() {
    console.log("销毁===============")
    this.webRtcServer.disconnect();
  }
}
</script>

<style>
</style>
