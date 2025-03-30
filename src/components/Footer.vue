<template>
  <footer class="site-footer">
    <div class="contact-info">
      Contact me at <a :href="'mailto:' + email">{{ email }}</a>.
    </div>
    <div class="social-links">
      <a :href="linkedinUrl" target="_blank" rel="noopener noreferrer">LinkedIn</a>
      <a :href="youtubeUrl" target="_blank" rel="noopener noreferrer">YouTube</a>
    </div>
  </footer>
</template>

<script setup>
import { ref } from 'vue';

const email = ref('johnmatthewtennant@gmail.com');
const linkedinUrl = ref('https://www.linkedin.com/in/johnmatthewtennant/');
const youtubeUrl = ref('https://www.youtube.com/channel/UCeMKK9VXp8mvs5tbeuRnPxg');
</script>

<style scoped>
.site-footer {
  margin-top: 40px;
  padding-top: 20px;
  border-top: 1px solid #ccc; /* Separator line */
  text-align: center;
  font-size: 0.9em;
  color: #555;
}

.site-footer div {
  margin-bottom: 10px;
}

.social-links a {
  margin: 0 10px; /* Space out social links */
  text-decoration: none;
  color: #007bff; /* Basic link color */
}

.social-links a:hover {
  text-decoration: underline;
}
</style>