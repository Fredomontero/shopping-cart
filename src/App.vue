<template>
  <Dashboard/>
</template>

<script>

import Dashboard from "./components/Dashboard.vue";

export default {
  name: 'App',
  components: {
    Dashboard
  }
}
</script>

<style>
#app {
  min-height: 100vh;
  height: 1px;
  border: 1px red solid;
  display: flex-block;
  flex-direction: column;
  align-items: center;
  padding: 50px;
  width: 100vw;
}
</style>
