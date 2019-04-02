<template>
  <div id="app">
    <div class="app-background"></div>
    <header class="app-header">LoCo Man Music</header>
    <div class="app-nav">
      <router-link to="/">Home</router-link>
    </div>
    <!-- -->
    <router-view/>
    <!-- -->
    <footer class="app-footer">1986 - {{ new Date().getFullYear() }} © LoCoMan</footer>
  </div>
</template>

<style lang="scss">
#app {
  position: relative;
  min-height: 100vh;
  // black background-color set in index.html body {}
  color: white;

  .app-background {
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
    width: 100%;
    height: 100%;
    background: url("./assets/images/app-background.gif")
      no-repeat center / cover;
    filter: blur(2px);
    opacity: 0.2;
  }

  .app-header {
    margin-bottom: 1rem;
    padding: 1rem 0;
    background-color: black;
    font-size: 40px;
    text-shadow: 0 1px 0 #e43526, 0 0 16px #e43526;
  }

  .app-nav {
    // router-link
    a {
      display: inline-block;
      margin-bottom: 1rem;
      color: white;
    }
  }

  .app-footer {
    position: fixed;
    left: 0;
    bottom: 0;
    padding: 0.66rem 0 0.5rem;
    width: 100%;
    background-color: black;
    font-size: 0.5rem;
  }
}
</style>
