<template>
  <div class="hello">
    <h1>Hello {{ msg }}</h1>
    <h2>{{ test }}</h2>
  </div>
</template>

<script>
export default {
  name: "Hello",
  data() {
    return {
      msg: "World",
      test: "message from Hello Component"
    };
  }
};
</script>
