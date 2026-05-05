<script setup>
import ChildComponent from './ChildComponent.vue';

const title2 = "Título del segundo hijo";

function displayMsg(msg) {
  alert(msg);
}
</script>

<template>
  <section class="parent-component">
    <h2>Este es el componente padre</h2>

    <ChildComponent title="Título del hijo 1" @send-msg="displayMsg">
      <p>Contenido HTML inyectado desde el padre al slot</p>
      <h5>Lorem ipsum dolor sit amet.</h5>

      <template #header>
        <h2>Este es el header del componente hijo</h2>
      </template>

      <template #footer>
        <h2>Footer del componente hijo</h2>
      </template>
    </ChildComponent>

    <ChildComponent :title="title2" />
  </section>
</template>

<style>
.parent-component {
  border: 2px dashed black;
  margin: 10px;
  padding: 5px;
}
</style>