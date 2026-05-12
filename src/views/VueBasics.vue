<script setup>
import ConditionalRendering from '@/components/ConditionalRendering.vue';
import ListRendering from '@/components/ListRendering.vue';
import ParentComponent from '@/components/ParentComponent.vue';
import ProductList from '@/components/ProductList.vue';
import VariablesComponent from '@/components/VariablesComponent.vue';

</script>

<template>
  <h2>Estos son los componentes básicos de Vue</h2>

  <ParentComponent />
  <VariablesComponent />
  <ConditionalRendering />
  <ListRendering />
  <ProductList />
</template>

<style></style>
