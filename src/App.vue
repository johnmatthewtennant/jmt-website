<template>
  <div>
    <Header />
    <Profile />
    <Compositions />
    <MusicVisualizers />
    <GuitarPlaying />
    <Footer />
  </div>
</template>

<script setup>
import Header from './components/Header.vue';
import Profile from './components/Profile.vue';
import Compositions from './components/Compositions.vue';
import MusicVisualizers from './components/MusicVisualizers.vue';
import GuitarPlaying from './components/GuitarPlaying.vue';
import Footer from './components/Footer.vue';
</script>

<style>
/* Add any global styles here if needed */
/* Let's add some basic centering and max-width like the old site */
body {
  font-family: sans-serif; /* Basic font */
}

div#app {
  max-width: 600px; /* Similar max-width */
  margin: 0 auto; /* Center the content */
  padding: 20px;
}
</style>