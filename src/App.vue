<template>
  <div id="app">
    <img width="25%" src="./assets/logo.png" />
    <hello-world />
    <hr />
    <div>test avec JS inheritance</div>
    <Hello />
    <hr />
    <div>test avec scope</div>
    <Hello> <hello-world slot-scope="hello" :message="hello.message" /> </Hello>
  </div>
</template>

<script>
import Vue from "vue";
import HelloWorld from "./components/HelloWorld";
import Hello from "./components/Hello";

export default {
  name: "App",
  components: {
    helloWorld: HelloWorld,
    Hello: Vue.extend(HelloWorld).extend(Hello)
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
