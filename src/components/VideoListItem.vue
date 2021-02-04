<script>
export default {
  name: 'VideoListItem',
  props: ['video']
};
</script>

<template>
    <li>
        {{video.snippet.title}}
    </li>
</template>