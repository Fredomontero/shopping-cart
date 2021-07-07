<template>
  <div class="dashboard-container">
    <h1>Shopping List</h1>
    <Input/>
    <ItemList/>
  </div>
</template>

<script>

import Input from './Input.vue';
import ItemList from "./ItemList.vue";

export default {
  name: 'Dashboard',
  components: {
    Input,
    ItemList
  }
}
</script>

<style scoped>
  .dashboard-container {
    font-family: 'Quicksand', sans-serif;
  }
</style>