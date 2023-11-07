<template>
  <h2>Name: {{ name }}</h2>
  <button v-on:click="changeName">Change Name</button>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "M Rizky Ferdiansyah",
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
