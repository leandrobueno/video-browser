<script>
import VideoListItem from "./VideoListItem";
export default {
  name: "VideoList",
  components: {
    VideoListItem,
  },
  props: {
    videos: Array,
  },
  data() {
    return {};
  },
};
</script>

<template>
  <ul>
      <VideoListItem 
        v-for="video in videos"
        :video="video"
        :key="video.etag">
      </VideoListItem>
  </ul>
</template>

<style scoped>
</style>