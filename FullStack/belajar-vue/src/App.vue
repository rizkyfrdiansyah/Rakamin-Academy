<template>
  <h2>Name: {{ name }}</h2>
  <button v-on:click="changeName">Ganti Nama</button>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "Muhammad Rizky Ferdiansyah",
    };
  },
  methods: {
    changeName() {
      this.name = "Bulskey";
    },
  },
};
</script>

<style></style>
