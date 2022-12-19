<template>
  <div>
    <iframe style="width: 640px;height:  480px;" name="ddddd" id="iframes" scrolling="auto"
            src="/static/test.html?data=rtsp://wowzaec2demo.streamlock.net/vod/mp4:BigBuckBunny_115k.mp4"></iframe>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tData: "123",
    }
  },
  mounted() {
    console.log("挂载==============")
  }
}
</script>

<style>
</style>
