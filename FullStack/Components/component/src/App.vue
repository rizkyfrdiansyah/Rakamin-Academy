<template>
  <!-- Output komponen Header -->
  <Header />
</template>

<script>
// Import komponen Header
import Header from "./components/Header.vue";

export default {
  name: "App",
  // Daftarkan komponen Header di components Property
  components: {
    Header,
  },
};
</script>

<style></style>
