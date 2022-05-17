<template>
  <div>
    <input type="text" v-model="todo" />
    <button v-on:click="handleClickRegister">登録</button>
    <p>入力内容: {{todo}}</p>
    <ul class="todoList">
      <li v-for="todo in todoList" v-bind:key="todo">{{todo}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'InputForm',
  data() {
    return {
      todo: '',
      todoList: []
    }
  },
  methods: {
    handleClickRegister(){
      console.log(this.todoList)
      this.todoList.push(this.todo)
    }
  }
}
</script>

<style scoped>
.todoList {
  padding: 5px;
  font-weight: bold;
}
</style>