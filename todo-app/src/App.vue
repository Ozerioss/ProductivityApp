<template>
  <div id="app">
    <todo-list v-bind:todos="todos"></todo-list>
  </div>
</template>


<script>

import TodoList from './components/TodoList'

export default {
  name: 'app',
  components: {
    TodoList
  },
  data () {
    return {
      todos: [{
        title: 'Test A',
        project: 'Test PR A',
        done: false
      },
      {
        title: 'Test B',
        project: 'Test PR B',
        done: true
      },
      {
        title: 'Test C',
        project: 'Test PR C',
        done: false
      }]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
