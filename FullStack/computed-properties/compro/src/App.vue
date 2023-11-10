<template>
  <!-- input search box -->
  <input type="text" v-model="search" placeholder="Search..." />
  <ul>
    <!-- loop data computed properties filterProducts -->
    <li v-for="product in filterProducts" v-bind:key="product.id">{{ product.title }} - {{ product.price }}</li>
  </ul>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      // data products
      search: "",
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
  // Computed Properties
  computed: {
    filterProducts() {
      // filter product dari array
      return this.products.filter((product) => {
        // Return title = search
        return product.title.match(this.search);
      });
    },
  },
};
</script>

<style></style>
