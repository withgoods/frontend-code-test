<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <custom-header title="Hello World" />
    <container
      :padding-top="isMobile ? '28px': '48px'"
      :padding-bottom="isMobile ? '0px': '48px'"
    >
    </container>

  <custom-main></custom-main>
  <custom-footer />
</template>

<script>
import CustomHeader from './components/custom/Header.vue'
import Container from './components/Container.vue'
import CustomMain from './components/custom/CustomMain.vue'
import CustomFooter from './components/custom/Footer.vue'

export default {
  components: {
    CustomHeader,
    Container,
    CustomMain,
    CustomFooter,
  },
  data() {
    return {}
  },
  props: {},
  methods: {},
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