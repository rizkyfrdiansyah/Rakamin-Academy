<template>
  <!-- jika ada data -->
  <div v-if="products.length">
    <ul>
      <!-- loop data -->
      <li v-for="product in products" v-bind:key="product.id">{{ product.title }} - {{ product.price }}</li>
    </ul>
  </div>
  <!-- jika tidak ada data -->
  <div v-else>
    <p>No data</p>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      // data products
      products: [], 
    };
  },
  // Created  Lifecycle Hooks
  created() {
    this.products = [
        { id: 1, title: "Product 1", price: 5000 },
        { id: 2, title: "Product 2", price: 4500 },
        { id: 3, title: "Product 3", price: 3700 },
        { id: 4, title: "Product 4", price: 1200 },
      ];
    },
};
</script>

<style></style>
