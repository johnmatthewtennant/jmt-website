<template>
  <section class="music-visualizers">
    <h2>Music Visualizers</h2>

    <div class="video-section">
      <h3>Cymatic Music Visualizer</h3>
      <div class="video-container">
        <iframe
          src="https://www.youtube.com/embed/_8fySo77IxM"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          referrerpolicy="strict-origin-when-cross-origin"
          allowfullscreen>
        </iframe>
      </div>
    </div>

    <div class="video-section">
      <h3>XY Oscilloscope Music Visualizer</h3>
      <div class="video-container">
        <iframe
          src="https://www.youtube.com/embed/IaS2guZumxI"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          referrerpolicy="strict-origin-when-cross-origin"
          allowfullscreen>
        </iframe>
      </div>
    </div>

  </section>
</template>

<script setup>
// No script logic needed yet
</script>

<style scoped>
.music-visualizers {
  margin-top: 40px;
  text-align: center;
}

h2 {
  margin-bottom: 20px;
}

.video-section {
  margin-bottom: 30px;
}

.video-section h3 {
  margin-bottom: 10px;
}

/* Responsive video container */
.video-container {
  position: relative;
  width: 100%;
  padding-bottom: 56.25%; /* 16:9 aspect ratio */
  height: 0;
  overflow: hidden;
  margin: 0 auto; /* Center container if needed */
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