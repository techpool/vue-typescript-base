<template>
  <div id="app">
    <TodoList 
      :todos="todos"
    />
  </div>
</template>

<script>
import TodoList from './components/TodoList.vue'

export default {
  name: 'App',
  components: {
    TodoList
  },
  data() {
    return {
      todos: [
        { id: 1, text: 'Learn Vue' },
        { id: 2, text: 'Learn Vue Router' },
        { id: 3, text: 'Learn Vuex' },
        { id: 4, text: 'Learn Nuxt' }
      ]
    }
  }
}
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
