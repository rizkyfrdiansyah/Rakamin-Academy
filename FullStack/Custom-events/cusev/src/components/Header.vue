<template>
  <!-- Output komponen Header -->
  <h2>{{ TextHeader }}</h2>
  <button v-on:click="changeText">Change Title</button>
</template>

<script>
export default {
  name: "Header",
  // Props Property
  props: ["TextHeader"],
  // Data Property
  data() {
    return {
      text: "Welcome To The Jungle",
    };
  },
  // Methods Property
  methods: {
    changeText() {
      this.$emit("changeTitle", this.text);
    },
  },
  // Emits Property
  emits: ["changeTitle"],
};
</script>

<style></style>
