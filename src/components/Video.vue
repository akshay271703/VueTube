<template>
  <div class="video">
    <img :src="video.img" :alt="video.title" />
    <div class="details">
      <p class="video-title">{{ video.title }}</p>
      <span class="uploader custom-text">{{ video.uploader }}</span>
      <span class="views custom-text">{{ video.views }} views</span>
      <span class="date custom-text">{{ video.date }} years ago</span>
    </div>
  </div>
</template>

<script>
export default {
  props: ["video"],
};
</script>

<style scoped>
.video img {
  width: 100%;
  height: auto;
}
.video {
  padding-bottom: 10px;
  max-height: 300px;
  width: 100%;
}

.video-title {
  margin-left: 20px;
  font-size: 16px;
  font-weight: 500;
  margin-bottom: 0;
}
.uploader {
  display: block;
  margin-top: 10px;
}
.custom-text {
  color: #999;
  margin-left: 20px;
  font-size: 13px;
  font-weight: 500;
  margin-bottom: 0;
}
</style>
