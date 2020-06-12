<template>
  <div>
    <nav>
      <router-link
        class="router"
        v-for="routes in links"
        v-bind:key="routes.id"
        :to="`${routes.page}`"
        >{{ routes.text }}</router-link
      >
    </nav>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Navigation extends Vue {
  private links: Array<object> = [
    {
      id: 1,
      text: "Home",
      page: "/"
    },
    {
      id: 2,
      text: "About",
      page: "/about"
    },
    {
      id: 3,
      text: "Contact",
      page: "/contact"
    }
  ];
}
</script>

<style>
.router {
  margin-right: 10px;
}
</style>
