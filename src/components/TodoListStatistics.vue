<template>
  <div>
    <h2>TodoListStatistics</h2>
    <h2>{{ todoLength }}</h2>
  </div>
</template>

<script>
export default {
  name: "TodoListStatistics",
  inject: ["todoLength"],
  created() {
    console.log(`Injected property: ${this.todoLength.value}`); // > Injected property: 5
  },
};
</script>

<style scoped>
</style>