<template>
<div id="app">
  <div id="nav">
    <div id="brand">
      <h1>The Event Place</h1>
    </div>
    <div id="links">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/schedule">Schedule</router-link>
    </div>
  </div>
  <router-view />
  <div id="footer"><a href="https://github.com/eworsham/cs260-creative-project-3" target="_blank">Github Repository</a></div>
</div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
