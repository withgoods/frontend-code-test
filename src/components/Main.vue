<template>
  <main>
    <div id="list-items-wrapper">
      <list-input :items="items"></list-input>
      <list-stats />
      <list-item
        v-for="item in items"
        :key="item"
        :item="item"
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
      items: [ 'Alfa', 'Bravo', 'Charlie', 'Delta', 'Echo' ]
    }
  },
};
</script>

<style lang="scss" scoped>
@import '../assets/scss/main.scss';
</style>
