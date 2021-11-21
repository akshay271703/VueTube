<template>
  <video width="800" height="500" autoplay controls>
    <source src="@/assets/demo.mp4" type="video/mp4" />
  </video>
</template>

<script>
export default {
  props: ["src"],
};
</script>

<style></style>
