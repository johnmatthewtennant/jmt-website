<template>
  <section class="compositions">
    <h2>Compositions</h2>
    <iframe
      style="border-radius:12px"
      src="https://open.spotify.com/embed/album/4QkYYBnQdSxcDEiZXhgrcI?utm_source=generator"
      width="100%"
      height="418"
      frameBorder="0"
      allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
      loading="lazy">
    </iframe>
    <!-- Optional: Add the 'Find on All Streaming Platforms' button later if desired -->
  </section>
</template>

<script setup>
// No script logic needed for this simple component yet
</script>

<style scoped>
.compositions {
  margin-top: 40px; /* Add some space above the section */
  text-align: center;
}

h2 {
  margin-bottom: 20px;
}

iframe {
  max-width: 100%; /* Ensure iframe is responsive */
}
</style>