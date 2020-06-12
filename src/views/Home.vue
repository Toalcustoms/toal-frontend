<template>
  <div class="home">
    <Navigation />
    <div>
      <h1>Home</h1>
      <p>Here is some information. This is the home page</p>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

import Navigation from "@/components/Navigation.vue";

@Component({
  components: {
    Navigation
  }
})
export default class Home extends Vue {}
</script>
