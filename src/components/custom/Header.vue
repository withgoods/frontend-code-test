<template>
  <header>
    <h1>{{ title }}</h1>
    <p>
      <a href="https://vitejs.dev/guide/features.html" target="_blank">Vite Documentation</a> |
      <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
    </p>
    <button @click="count++">count is: {{ count }}</button>
  </header>
</template>

<script>
export default {
  data() {
    return {
      count: 0
    }
  },
  props: {
    title: {
      type: String,
      default: 'Vue.js Code Testing Page',
    }
  },
};
</script>

<style lang="scss" scoped>
a {
  color: #42b983;
}
</style>
