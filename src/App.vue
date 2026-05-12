<script setup>
import HeaderComponent from './components/HeaderComponent.vue';

</script>

<template>
  <HeaderComponent />

  <RouterView />
</template>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
}
</style>
