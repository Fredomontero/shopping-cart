<template>
  <div class="dashboard-container">
    <h1>Shopping List</h1>
    <Input v-if="showInputField"/>
    <button @click="toggleInputField" class="add-btn">+</button>
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
  },
  data(){
    return {
      showInputField: false
    }
  },
  methods: {
    toggleInputField(){
      this.showInputField = !this.showInputField;
    }
  }
}
</script>

<style scoped>
  .dashboard-container {
    font-family: 'Quicksand', sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .dashboard-container h1 {
    font-size: 35px;
    font-weight: 400;
  }

  .add-btn {
    position: absolute;
    background-color: #cd5c5c;
    border-radius: 25px;
    font-size: 30px;
    color: #fff;
    height: 50px;
    width: 50px;
    border: none;
    bottom: 30px;
    right: 30px;
    cursor: pointer;
  }
</style>