<template>
  <nav class="top-navigation">
    <div class="top-navigation__logo">
      <img src="@/assets/logo.png" alt="logo" />
    </div>
    <div class="top-navigation__links">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
      <router-link to="/about">{{ dupa }}</router-link>
    </div>
  </nav>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    dupa: String,
  },
})
export default class BaseNavigation extends Vue {
  dupa!: string;
}
</script>

<style lang="scss">
@import "@/scss/_variables.scss";

.top-navigation {
  display: grid;
  grid-template-columns: 100px auto;
  padding: $screen-gutter-mobile;
  background-color: transparent;
}
</style>
