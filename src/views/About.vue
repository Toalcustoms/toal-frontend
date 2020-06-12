<template>
  <div class="about">
    <Navigation />
    <div>
      <h1>About</h1>
      <p>Here is some information. This is the about page</p>
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
export default class About extends Vue {}
</script>
