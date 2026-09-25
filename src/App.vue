<script setup>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
import { RouterView } from "vue-router";
</script>

<template>
  <div class="app-shell">
    <Navbar />
    <main class="page-content">
      <RouterView />
    </main>
    <Footer />
  </div>
</template>

<style scoped>
.app-shell {
  min-height: 101vh;
  display: flex;
  flex-direction: column;
}

.page-content {
  flex: 1;
  width: min(1200px, calc(100% - 32px));
  margin: 0 auto;
}
</style>
