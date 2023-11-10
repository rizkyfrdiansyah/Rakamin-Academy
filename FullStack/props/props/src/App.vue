<template>
  <!-- Bind Props ke komponen Header -->
  <Header v-bind:TextHeader="text" />
</template>

<script>
import Header from "./components/Header.vue";
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: "App",
  components: {
    Header,
  },
  // data property
  data() {
    return {
      text: "Welcome To Bulskey",
    };
  },
};
</script>

<style></style>
