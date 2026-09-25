<template>
  <header class="topbar">
    <nav class="nav">
      <h2 class="brand">SMK Yadika Soreang - Onlineshop</h2>
      <div class="nav-links">
        <RouterLink to="/">Landing</RouterLink>
        <RouterLink to="/product">Product</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/contact" class="active">Contact</RouterLink>
      </div>
    </nav>
  </header>
</template>

<style scoped>
.topbar {
  background: #fff;
  border-bottom: 1px solid #f3d3dc;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.03);
}

.nav {
  width: min(1200px, calc(100% - 32px));
  margin: 0 auto;
  padding: 18px 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 16px;
}

.brand {
  font-size: 1.15rem;
  color: #2c3e50;
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 14px;
  flex-wrap: wrap;
}

.nav-links a {
  color: #2c3e50;
  font-weight: 600;
  padding: 8px 12px;
  border-radius: 999px;
}

.nav-links a:hover,
.nav-links a.router-link-active {
  background: #ffe4ea;
  color: #d63c5a;
}
</style>
