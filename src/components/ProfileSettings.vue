<template>
  <div class="my-profile">
    <HeaderProfile />
    <MyProfile />
  </div>
</template>

<script setup>
import HeaderProfile from './HeaderProfile.vue'
import MyProfile from './MyProfile.vue'
</script>

<style scoped>
.my-profile {
  display: flex;
  flex-direction: column;
  width: 100%;
}
</style>
