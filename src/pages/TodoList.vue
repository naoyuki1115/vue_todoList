<template>
  <div id="todoList">
    <img alt="Vue logo" src="../assets/logo.png">
    <h1>{{title}}</h1>
    <TodoForm/>
  </div>
</template>

<script>
import TodoForm from "../components/TodoForm.vue"

export default {
  name: 'TodoList',
  components: {
    TodoForm
  },
  props: {
    title: String
  },
}
</script>

<style>
#todoList {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
