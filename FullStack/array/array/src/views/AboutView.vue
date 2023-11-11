<template>
  <div class="about">
    <h1>This is an about page</h1>

    <div>
      <ol>
        <li v-for="(food, index) in foods" :key="index">
          {{ food }}
        </li>
      </ol>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      foods: ["Nasi Goreng", "Lontong Sayur", "Bakso", "Mie Ayam", "Ketoprak"],
    };
  },
};
</script>
