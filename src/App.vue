<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <GetName/>
</template>

<script>
import GetName from "./components/GetName.vue";

export default {
    name: "App",
    components: { GetName }
}
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
