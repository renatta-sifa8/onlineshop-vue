<script setup>
const tahun = new Date().getFullYear();
</script>

<template>
  <footer class="site-footer">
    <small>&copy; {{ tahun }} SMK Yadika Soreang — Onlineshop Sekolah</small>
  </footer>
</template>

<style scoped>
.site-footer {
  padding: 20px 16px 28px;
  text-align: center;
  color: #5e6475;
  background: #fff;
  border-top: 1px solid #f3d3dc;
}
</style>
