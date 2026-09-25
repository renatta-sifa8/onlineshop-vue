<script setup>
import ProductCard from "../components/ProductCard.vue";

const daftarProduk = [
  {
    id: 1,
    nama: "kos kaki",
    harga: 100000,
    gambar: "kos kaki.jpg",
  },
  {
    id: 2,
    nama: "topi",
    harga: 3000000,
    gambar: "topi.jpg",
  },
  {
    id: 3,
    nama: "Tas",
    harga: 2000000,
    gambar: "tas sekolah.jpg",
  },
];
</script>

<template>
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 p-6">
    <ProductCard
      v-for="produk in daftarProduk"
      :key="produk.id"
      :nama="produk.nama"
      :harga="produk.harga"
      :gambar="produk.gambar"
    />
  </div>
</template>

<style scoped>
.product-page {
  padding: 2rem 0 3rem;
}

.product-page h1 {
  margin-bottom: 1.5rem;
  color: #2c3e50;
}

.grid {
  display: flex;
  flex-wrap: wrap;
  gap: 18px;
}
</style>
