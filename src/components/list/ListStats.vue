<template>
  <div class="item">
    <p>Todos: {{ todos.length }}</p>
  </div>
</template>

<script>
      
export default {
  components: {},
  data() {
    return { isChecked: false }
  },
  props: {
    todo: {
      type: String,
      default: '',
    },
    todos: {
      type: Array,
      default: [],
    },
  },
  methods: {
    removeItem: function(todo) {
      let trashedItemIndex = this.todos.indexOf(todo)
      this.todos.splice(trashedItemIndex, 1)
    }
  },
};
</script>

<style lang="scss" scoped>
@import '../component-styles.scss';
</style>
