<template>
  <div class="video-grid-body">
    <div class="videos">
      <Video v-for="video in data" :key="video.id" :video="video" />
    </div>
  </div>
</template>

<script>
import Video from "@/components/Video.vue";
import data from "@/assets/dummyData";
export default {
  components: {
    Video,
  },
  data: () => {
    return {
      data: data,
    };
  },
};
</script>

<style scoped>
.video-grid-body {
  min-height: 100vh;
  background-color: #f9f9f9;
  width: 100%;
  margin-top: 55px;
  margin-left: 80px;
  padding: 20px;
}
.videos {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-gap: 20px;
}
</style>
