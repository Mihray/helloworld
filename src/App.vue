<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <GetName/>
  <SignLogin/>
  <DlrowOlloeh/>
  <MonitorVue/>
  <DetectiveVue/>
  <ListVue/>
  <TwowayDataBinding/>
  <DlrowOlloeh/>
</template>

<script>
import GetName from "./components/GetName.vue";
import SignLogin from "./components/SignLogin.vue";
import DlrowOlloeh from "./components/DlrowOlloeh.vue";
import MonitorVue from "./components/MonitorVue.vue";
import DetectiveVue from "./components/DetectiveVue.vue";
import ListVue from "./components/ListVue.vue";
import TwowayDataBinding from "./components/TwowayDataBinding.vue";

export default {
    name: "App",
    components: { GetName, SignLogin, DlrowOlloeh, MonitorVue, DetectiveVue,ListVue,TwowayDataBinding }
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
