<template>
  <header class="app__header">
    <nav class="app__navbar">
      <div class="app__navbar__left">
        <img class="app__navbar__logo" src="./assets/logo.png" alt="logo" />
        <h1 class="app__navbar__title">차트로 보는 코로나 현황</h1>
      </div>
      <p>v1.0.0</p>
    </nav>
  </header>
  <router-view></router-view>
  <footer class="app__footer">
    <p>
      Cocha developed by
      <a href="https://github.com/cre4tive97/Cocha">@cre4tive97</a>
    </p>
  </footer>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>
@import url("./assets/reset.css");
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: black;
}
.app__header {
  padding: 8px 16px;
  background: #005ecb;
  color: white;
}
.app__navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.app__navbar__left {
  display: flex;
  align-items: center;
}
.app__navbar__title {
  font-size: 1.3rem;
}
.app__navbar__logo {
  width: 40px;
  margin-right: 1rem;
}
.app__footer {
  position: fixed;
  bottom: 4px;
  font-size: 0.75rem;
  right: 4px;
  font-weight: 500;
  display: flex;
  color: black;
}
.app__footer a {
  color: black;
  text-decoration: none;
}
</style>
