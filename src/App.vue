<template>
  <div id="app" class="pure-g">
    <div id="nav" class="pure-u-5-5">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view class="pure-u-5-5 page-container"/>
  </div>
</template>

<style lang="scss">
@import '../node_modules/purecss/build/pure-min.css';
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
html, body {
  height: 100%;
  background-color: #5E5D5D
}
</style>
