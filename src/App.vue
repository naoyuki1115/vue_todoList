<template>
  <div>
    <TodoList title="Vue ToDo List"/>
  </div>
</template>

<script>
import TodoList from "./pages/TodoList.vue"

export default {
  name: 'App',
  components: {
    TodoList
  }
}
</script>

<style>

</style>
