<template>
  <div class="profile-container">
    <img :src="profileImageUrl" alt="Profile Picture" class="profile-picture">
  </div>
</template>

<script setup>
import { ref } from 'vue';
// Use url: prefix to ensure Parcel resolves the path correctly
import profileImage from 'url:../../assets/profile.jpg';

const profileImageUrl = ref(profileImage);
</script>

<style scoped>
.profile-container {
  text-align: center;
  margin: 30px auto; /* Add some margin above/below and center */
}

.profile-picture {
  width: 250px; /* Increased size */
  height: 250px; /* Increased size */
  border-radius: 50%;
  object-fit: cover;
}
</style>