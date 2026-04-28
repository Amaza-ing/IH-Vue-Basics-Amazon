<script setup>
import ConditionalRendering from './components/ConditionalRendering.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import ListRendering from './components/ListRendering.vue';
import ProductList from './components/ProductList.vue';
import VariablesComponent from './components/VariablesComponent.vue';

</script>

<template>
  <HeaderComponent />

  <VariablesComponent />
  <ConditionalRendering />
  <ListRendering />
  <ProductList />
</template>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
}
</style>
