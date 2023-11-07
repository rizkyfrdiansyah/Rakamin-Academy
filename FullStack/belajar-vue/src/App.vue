<template>
  <a v-bind:href="url">GO TO BULSKEY.COM</a>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      url: "https://bulskey.com",
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
