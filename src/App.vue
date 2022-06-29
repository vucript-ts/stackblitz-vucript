<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Welcome to Your Vue.js + Vucript App" />
  <button @click="increment">count is: {{ count }}</button>
</template>

<script lang="vucript">
import { importComponent,reactive } from 'vucript'
importComponent('./components/HelloWorld.vue','HelloWorld');
let count:reactive<number> = 0;
let increment=()=>{
  count++;
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
