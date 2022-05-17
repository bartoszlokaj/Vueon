<template>
  <nav>
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
  </nav>
  <router-view />
</template>

<style lang="scss" global>
@import "@/scss/_colors.scss";
body {
  background-color: $color-primary;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $color-secondary;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: $color-secondary;

    &.router-link-exact-active {
      color: $color-primary;
    }
  }
}
</style>
