<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
html {
  height: 100%;
}
body {
  height: 100%;
  background: #387cc2 url() 50% 50% no-repeat;
  background-size: cover;
}
#app{
  height: 100%;
}
</style>
