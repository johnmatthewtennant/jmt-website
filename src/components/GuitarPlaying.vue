<template>
  <section class="guitar-playing">
    <h2>Guitar Playing</h2>
    <div class="video-container">
      <iframe
        :src="videoUrl"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        referrerpolicy="strict-origin-when-cross-origin"
        allowfullscreen>
      </iframe>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';

// Extract video ID from the provided watch link
const videoId = 'coTYT_OX9iA';
const videoUrl = ref(`https://www.youtube.com/embed/${videoId}`);
</script>

<style scoped>
.guitar-playing {
  margin-top: 40px;
  text-align: center;
}

h2 {
  margin-bottom: 20px;
}

/* Reusing the responsive video container styles */
.video-container {
  position: relative;
  width: 100%;
  padding-bottom: 56.25%; /* 16:9 aspect ratio */
  height: 0;
  overflow: hidden;
  margin: 0 auto;
  max-width: 100%;
}

.video-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>