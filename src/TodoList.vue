<template>
  <div id="app">
    <TodoListFooter />
  </div>
</template>

<script>
import TodoListFooter from "./components/TodoListFooter";

export default {
  name: "App",
  components: {
    TodoListFooter,
  },
  data() {
    return {
      todos: ["Feed a cat", "Buy tickets"],
    };
  },
  provide() {
    return {
      todoLength: this.todos.length,
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
