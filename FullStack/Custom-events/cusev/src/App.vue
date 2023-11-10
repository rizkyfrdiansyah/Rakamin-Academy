<template>
  <!-- Output komponen Header -->
  <Header @changeTitle="changeTitle" v-bind:TextHeader="text" />
</template>

<script>
// Import komponen Header
import Header from "./components/Header";

export default {
  name: "App",
  components: {
    Header,
  },
  // Data Property
  data() {
    return {
      text: "Welcome To M Fikri",
    };
  },
  // Methods Property
  methods: {
    changeTitle(newTitle) {
      this.text = newTitle;
    },
  },
};
</script>

<style></style>
