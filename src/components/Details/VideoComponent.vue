<template>
  <div class="video-component-body">
    <div class="video">
      <VideoPlayer />
      <VideoDetail />
      <VideoComments />
    </div>
  </div>
</template>

<script>
import VideoPlayer from "@/components/Video/VideoPlayer.vue";
import VideoDetail from "@/components/Video/VideoDetail.vue";
import VideoComments from "@/components/Video/VideoComments.vue";
export default {
  components: {
    VideoPlayer,
    VideoDetail,
    VideoComments,
  },
  props: ["video"],
};
</script>

<style scoped>
.video-component-body {
  margin-left: 80px;
}
.video {
  max-width: 800px;
}
</style>
