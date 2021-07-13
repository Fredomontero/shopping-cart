<template>
  <div class="item-container">
    <div>{{ item.name }}</div>
    <div class="icons">
      <div class="check-icon">
        <i class="fas fa-check"></i>
      </div>
      <div class="delete-icon">
        <i class="fas fa-trash"></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Item',
  props: {
    item: Object
  }
}
</script>

<style scoped>
  .item-container {
    border: 1px solid #000;
    padding: 10px;
    justify-content: space-between;
    align-items: center;
    display: flex;
    font-size: 25px;
    height: 75px;
    width: 400px;
    margin: 20px 0;
  }

  .icons {
    width: 35%;
    display: flex;
    justify-content: space-between;
    vertical-align: middle;
  }

  .check-icon{
    background-color: #71bc78;
    color: #fff;
    width: 60px;
    height: 40px;
    text-align: center;
  }

  .check-icon i{
    width: 40px;
    height: 40px;
    position:relative;
    top: calc(50% - 15px);
  }

  .delete-icon{
    background-color: #ff2052;
    color: #fff;
    width: 60px;
    height: 40px;
    text-align: center;

  }

  .delete-icon i{
    width: 40px;
    height: 40px;
    position:relative;
    top: calc(50% - 15px);
  }
</style>