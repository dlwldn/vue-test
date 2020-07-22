<template>
  <div id="app">
    <h1>안녕 ~!</h1>
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Vue 테스트" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #0066ff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
