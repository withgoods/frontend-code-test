<template>
  <div class="item">
    <p>Add item</p>
    <input type="text" v-model="userInput" v-on:keydown.enter="addItem"/>
    <div class="plus-circle-svg svg-wrapper" v-on:click="addItem">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"></circle><line x1="12" y1="8" x2="12" y2="16"></line><line x1="8" y1="12" x2="16" y2="12"></line></svg>
    </div>
  </div>
</template>

<script>
      
export default {
  data() {
    return { userInput: "" }
  },
  methods: {
    addItem() {}
  },
};
</script>

<style lang="scss" scoped>
@import '../../assets/scss/main.scss';
</style>
