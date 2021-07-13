<template>
  <div class="item-container">
    <Item v-for="product in products" :key="product.id" :item="product" />
  </div>
</template>

<script>

import Item from './Item.vue';

export default {
  name: 'ItemList',
  props: {
    products: Array
  },
  components: {
    Item
  }
}
</script>

<style scoped>

</style>