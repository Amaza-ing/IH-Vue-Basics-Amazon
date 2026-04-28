<script setup>
import { ref } from 'vue';

const isLoggedIn = ref(false);

function login() {
  isLoggedIn.value = true;
}

function logout() {
  isLoggedIn.value = false;
}
</script>

<template>
  <p v-if="isLoggedIn">Bienvenido usuario!</p>
  <p v-else>Necesitas hacer login.</p>

  <button v-if="!isLoggedIn" @click="login">Login</button>
  <button v-else @click="logout">Log out</button>
</template>

<style></style>