<template>
  <div class="layout">
    <header class="header">
      <Navbar />
      <div class="uk-container"></div>
    </header>
    <div class="uk-container">
      <slot />
    </div>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>
<script>
import Navbar from "~/components/Navbar.vue";
export default {
  components: {
    Navbar
  }
};
</script>
<style></style>
