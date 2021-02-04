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
  methods: {
      videoSelect() {

      }
  }
};
</script>

<template>
  <ul class="list-group">
      <VideoListItem      
        v-for="video in videos"
        :video="video"
        :key="video.etag"
        @videoSelect="videoSelect">
      </VideoListItem>
  </ul>
</template>

<style scoped>

</style>