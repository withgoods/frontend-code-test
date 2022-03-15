<template>
  <img alt="Vue logo" src="./assets/images/logo.png" />
  <custom-header />
  <custom-main />
  <custom-footer />
</template>

<script>
import CustomHeader from './components/custom/Header.vue'
import CustomMain from './components/Main.vue'
import CustomFooter from './components/custom/Footer.vue'

export default {
  components: {
    CustomHeader,
    CustomMain,
    CustomFooter,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>