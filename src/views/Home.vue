<template>
  <div class="home">
    <div class="container">
      <AddTodo/>
      <FilterTodos/>
      <Todos/>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Todos from "../components/Todos.vue";
import AddTodo from "../components/AddTodo.vue";
import FilterTodos from "../components/FilterTodos.vue";

export default {
  name: "home",
  components: {
    Todos,
    AddTodo,
    FilterTodos
  }
};
</script>

<style scoped>
.home {
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
  line-height: 1.6;
  background: #e8f7f0;
}

.container {
  max-width: 1100px;
  margin: auto;
  overflow: auto;
  padding: 0 2rem;
}
</style>

