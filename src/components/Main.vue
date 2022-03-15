<template>
  <main>
    <div id="list-items-wrapper">
      <list-input :todos="todos"></list-input>
      <list-stats :todos="todos"></list-stats>
      <list-item
        v-for="todo in todos"
        :key="todo"
        :todo="todo"
        :todos="todos"
      >
      </list-item>
    </div>
  </main>
</template>

<script>
import ListInput from './list/ListInput.vue'
import ListStats from './list/ListStats.vue'
import ListItem from './list/ListItem.vue'

export default {
  components: {
    ListInput,
    ListStats,
    ListItem,
  },
  data() {
    return {
      todos: [ 'Alfa', 'Bravo', 'Charlie', 'Delta', 'Echo' ]
    }
  },
};
</script>

<style lang="scss" scoped>
@import '../assets/scss/main.scss';
</style>
