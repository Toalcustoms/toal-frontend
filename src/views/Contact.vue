<template>
  <div class="contact">
    <Navigation />
    <div>
      <h1>Contact Us</h1>
      <ul>
        <li>Email: {{ email }}</li>
        <li>Website: {{ web }}</li>
      </ul>
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
export default class Contact extends Vue {
  private email = "contact@toalcustoms.com";
  private web = "toalcustoms.com";
}
</script>
