<template>
  <header>
    <h1>{{ title }}</h1>
    <p>
      <a href="https://vitejs.dev/guide/features.html">Vite Documentation</a> |
      <a href="https://v3.vuejs.org/">Vue 3 Documentation</a>
    </p>
    <button>count is: 0</button>
  </header>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Hello World',
    }
  },
};
</script>

<style lang="scss" scoped>
a {
  color: #42b983;
}
</style>
