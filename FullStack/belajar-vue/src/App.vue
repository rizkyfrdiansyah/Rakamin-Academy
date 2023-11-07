<template>
  <input type="text" v-model="name" />
  <h4>Name: {{ name }}</h4>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "",
    };
  },
};
</script>
