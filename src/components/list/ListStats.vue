<template>
  <div class="item">
    <p>Number of List: {{ todos.length }}</p>
  </div>
</template>

<script>
      
export default {
  props: {
    todos: {
      type: Array,
      default: [],
    },
  },
};
</script>

<style lang="scss" scoped>
@import '../../assets/scss/main.scss';
</style>
