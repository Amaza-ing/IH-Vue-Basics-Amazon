<script setup>
const props = defineProps({
  product: Object,
});

const emit = defineEmits([
  "delete",
])

function deleteProduct() {
  emit("delete", props.product.id);
}
</script>

<template>
  <article class="product-card">
    <h3 class="product-name">{{ props.product.name }}</h3>
    <img :src="props.product.img" alt="imagen del producto" width="100" />
    <h4>{{ props.product.price }}€</h4>
    <button @click="deleteProduct">Eliminar</button>
  </article>
</template>

<style>
.product-card {
  width: 150px;
  height: 250px;
  background-color: lightgray;
  padding: 5px 15px;
  margin: 10px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;

  .product-name {
    font-size: 28px;
  }
}
</style>
