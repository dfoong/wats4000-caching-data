<template>
  <div id="app">
    <h1>Weather Service</h1>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #52a7c2;
  width: 75%;
  margin: 20px auto;
}
</style>
