<template>
  <div>
    <h1>This is ComponentA</h1>
    <p>Name: {{ username }}</p>
    <p>______________________</p>
    <ComponentB />
  </div>
</template>

<script>
import ComponentB from "./ComponentB.vue";
export default {
  name: "ComponentA",
  components: {
    ComponentB,
  },
  inject: ["username"],
};
</script>

<style>
</style>