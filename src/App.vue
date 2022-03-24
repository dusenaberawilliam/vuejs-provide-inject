<template>
  <div id="app">
    <h1>This is AppComponent</h1>
    <p>Name: {{ name }}</p>
    <p>______________________</p>
    <ComponentA />
  </div>
</template>

<script>
import ComponentA from "./components/ComponentA";
export default {
  name: "App",
  components: {
    ComponentA,
  },
  data() {
    return {
      name: "William",
    };
  },
  provide() {
    return {
      username: this.name,
    };
  },
};
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
