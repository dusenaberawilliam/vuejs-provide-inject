<template>
  <div>
    <h1>This is ComponentC</h1>
    <p>Name: {{ username }}</p>
    <p>______________________</p>
  </div>
</template>

<script>
export default {
  name: "ComponentC",
  inject: ["username"],
};
</script>

<style>
</style>