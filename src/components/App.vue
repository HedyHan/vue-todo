<template>
  <div id="app">
    <h1>{{ msg }}</h1>
    <TodoList></TodoList>
  </div>
</template>

<script>
  import TodoList from "./TodoList.vue";

  export default {
    name: 'app',
    components: {
        TodoList
    },
    data () {
      return {
        msg: 'Todo List'
      }
    }
  }
</script>

<style scoped>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin-top: 60px;
  }

  img {
    width: 200px;
    height: 200px;
  }

  h1, h2 {
    font-weight: normal;
  }
</style>
