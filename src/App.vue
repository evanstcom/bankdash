<script setup>
import NavigationMenu from './components/NavigationMenu.vue'
import ProfileSettings from './components/ProfileSettings.vue'
</script>

<template>
  <main class="wrapper">
    <NavigationMenu />
    <ProfileSettings />
  </main>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

a {
  text-decoration: none;
}

.wrapper {
  display: flex;
  width: 100%;
}
</style>
