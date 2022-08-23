<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <GetName/>
  <SignLogin/>
  <DlrowOlloeh/>
</template>

<script>
import GetName from "./components/GetName.vue";
import SignLogin from "./components/SignLogin.vue";
import DlrowOlloeh from "./components/DlrowOlloeh.vue";

export default {
    name: "App",
    components: { GetName, SignLogin, DlrowOlloeh }
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
