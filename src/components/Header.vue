<template>
  <header class="site-header">
    <h1>{{ name }}</h1>
    <p>Contact me at <a :href="'mailto:' + email">{{ email }}</a>.</p>
    <hr class="separator">
  </header>
</template>

<script setup>
import { ref } from 'vue';

const name = ref('John Matthew Tennant');
const email = ref('johnmatthewtennant@gmail.com');
</script>

<style scoped>
.site-header {
  text-align: center;
  margin-bottom: 20px;
}

h1 {
  font-size: 2.5em; /* Adjust as needed */
  margin-bottom: 0.5em;
}

.separator {
  border: 0;
  height: 1px;
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0));
  margin-top: 20px;
  margin-bottom: 20px;
}
</style>