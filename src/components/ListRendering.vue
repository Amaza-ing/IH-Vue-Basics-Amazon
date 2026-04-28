<script setup>
const names = ["Ana", "Ana", "Beatriz", "Carlos", "David", "Elena"];
</script>

<template>
  <ul>
    <li v-for="(name, index) in names" :key="index">
      {{ index }} {{ name }}
    </li>
  </ul>
</template>

<style></style>