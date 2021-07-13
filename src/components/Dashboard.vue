<template>
  <div class="dashboard-container">
    <h1>Shopping List</h1>
    <Input v-if="showInputField"/>
    <button v-if="showInputField" @click="toggleInputField" class="close-btn">×</button>
    <button v-else @click="toggleInputField" class="add-btn">+</button>
    <ItemList :products="products"/>
  </div>
</template>

<script>

import Input from './Input.vue';
import ItemList from "./ItemList.vue";

import { products } from '../data';

export default {
  name: 'Dashboard',
  components: {
    Input,
    ItemList
  },
  data(){
    return {
      showInputField: false,
      products: products
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
    margin-bottom: 30px;
  }

  .add-btn {
    position: fixed;
    background-color: #00a86b;
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

  .close-btn {
    position: fixed;
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