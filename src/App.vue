<template>
  <div id="app">
    <Topbar v-bind:msg="msg" />
    {{msg}}
    <br />
    제이름은: {{name}}
    <br />
    <br />
    <input type="text" v-model="name" />
    <label>제목</label>
    <input type="text" v-model="msg" />
    <Bottom />
  </div>
</template>

<script>
import Topbar from "./components/Topbar.vue";
import Bottom from "./components/Bottom.vue";

export default {
  name: "App",
  components: {
    Topbar,
    Bottom
  },
  data() {
    return {
      msg: "Hello Vue JS",
      name: ""
    };
  }
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

body {
  width: 100%;
  height: 100vh;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #0066ff;
}

input {
  width: 200px;
  height: 30px;
  border-radius: 10px;
  border: 1px solid gray;
}

.header {
  background-color: crimson;
  height: 100px;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 3rem;
  margin-bottom: 30px;
}

.footer {
  background-color: #333;
  height: 100px;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 3rem;
  margin-top: 30px;
  position: fixed;
  bottom: 0;
  width: 100%;
}
</style>
