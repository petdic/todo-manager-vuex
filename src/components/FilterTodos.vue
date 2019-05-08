<template>
  <div>
    Filter Todos:
    <select v-on:change="filterTodos($event)">
      <option value="200">200</option>
      <option value="50">100</option>
      <option value="10">10</option>
      <option value="5">5</option>
    </select>
  </div>
</template>

<script>
import { mapActions } from "vuex";

export default {
  name: "FilterTodos",
  methods: mapActions(["filterTodos"])
};
</script>

<style scoped>
select {
  margin-top: 20px;
  padding: 6px;
  border: 1px solid #41b883;
}
</style>
