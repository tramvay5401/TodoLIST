<template>
  <div id="app">
  <h1>SIMPLE TODO LISTS</h1>
  <TodoList
          v-bind:todos="todos"
  />
  </div>
</template>

<script>
import TodoList from "@/components/TodoList";

export default {

  name: "app",
  data(){
    return{
      todos:[
        {id: 1, title:'go to work', completed:false },
        {id: 1, title:'go to work', completed:false },
        {id: 1, title:'go to work', completed:false }
      ]
    }
  },
  components: {
    TodoList
}
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
