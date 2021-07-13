<template>
  <div class="input-container">
    <input type="text" placeholder="Add new Item">
    <button>Add</button>
  </div>
</template>

<script>
export default {
  name: 'Input'
}
</script>

<style scoped>
  .input-container {
    margin-bottom: 30px;
    border: 1px solid #888888;
    height: 50px;
    width: 70%;
    padding: 3px;
    border-radius: 5px;
    box-shadow: 5px 10px 18px #888888;
  }

  .input-container input {
    width: 95%;
    height: 100%;
    font-size: 20px;
    border-radius: 5px;
    border: none;
    padding: 0px 5px;
  }

  .input-container input:focus {
    outline: none;
    border: none;
  }

  .input-container button {
    width: 5%;
    height: 100%;
    background-color: #00a86b;
    color: #fff;
    border: none;
    font-size: 20px;
    border-radius: 5px
  }

</style>