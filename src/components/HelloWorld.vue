<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>{{ message }}</h2>
    <h3>message from HelloWorld Component</h3>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    message: {
      type: String,
      default: "message from HelloWorld Component"
    }
  },
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  color: tomato;
  font-weight: normal;
}
</style>
