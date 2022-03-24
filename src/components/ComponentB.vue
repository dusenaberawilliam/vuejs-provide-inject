<template>
  <div>
    <h1>This is ComponentB</h1>
    <p></p>
    <p>______________________</p>
    <ComponentC />
  </div>
</template>

<script>
import ComponentC from "./ComponentC.vue";
export default {
  name: "ComponentB",
  components: {
    ComponentC,
  },
};
</script>

<style>
</style>