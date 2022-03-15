<template>
    <container
      :padding-top="isMobile ? '28px': '48px'"
      :padding-bottom="isMobile ? '0px': '48px'"
    >
    </container>

  <CustomMain></CustomMain>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3 + Vite" />
</template>

<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Container from './components/Container.vue'
import CustomMain from './components/custom/CustomMain.vue'
  
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