<template>
  <div id="app">
    <h1>{{ msg }}</h1>
    <TodoInput></TodoInput>
    <TodoList></TodoList>
  </div>
</template>

<script>
  import TodoInput from "./TodoInput.vue";
  import TodoList from "./TodoList.vue";

  export default {
    name: 'app',
    components: {
        TodoInput,
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
    text-align: center;
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

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>
