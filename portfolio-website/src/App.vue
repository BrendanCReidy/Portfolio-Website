<template>
  <router-view/>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  background-color: #444d69;
}
body {
    background-color: #444d69;
}
.container:nth-child(odd) {
    background-color: #444d69;
}
.container:nth-child(even) {
    background-color: #949cb1;
}
</style>
