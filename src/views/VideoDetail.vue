<template>
  <div class="video-detail-body">
    <Sidebar />
    <VideoComponent />
  </div>
</template>

<script>
import Sidebar from "@/components/Sidebar.vue";
import VideoComponent from "@/components/Details/VideoComponent.vue";
export default {
  components: {
    Sidebar,
    VideoComponent,
  },
};
</script>

<style></style>
