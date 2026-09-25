<template>
  <div class="contact-page">
    <section class="hero-banner">
      <h1>contect us</h1>
    </section>

    <main class="content-container">
      <div class="contact-grid">
        <div class="contact-info">
          <h2>Info Kontak</h2>
          s

          <div class="info-item">
            <div class="info-header">
              <span class="icon">📍</span>
              <strong>Alamat</strong>
            </div>
            <p>Jl. Pendidikan No. 1, Soreang, Kab. Bandung</p>
          </div>

          <div class="info-item">
            <div class="info-header">
              <span class="icon">📞</span>
              <strong>Telepon</strong>
            </div>
            <p>(022) 123 4567</p>
          </div>

          <div class="info-item">
            <div class="info-header">
              <span class="icon">✉️</span>
              <strong>Email</strong>
            </div>
            <p>onlineshop@smkyadikasoreang.sch.id</p>
          </div>
        </div>

        <div class="contact-form-section">
          <h2>Kirim Pesan</h2>

          <form @submit.prevent="handleSubmit" class="contact-form">
            <div class="form-group">
              <label for="name">Nama</label>
              <input
                type="text"
                id="name"
                v-model="formData.name"
                placeholder="Nama Anda"
                required
              />
            </div>

            <div class="form-group">
              <label for="email">Email</label>
              <input
                type="email"
                id="email"
                v-model="formData.email"
                placeholder="email@contoh.com"
                required
              />
            </div>

            <div class="form-group">
              <label for="message">Pesan</label>
              <textarea
                id="message"
                v-model="formData.message"
                placeholder="Tulis pesan..."
                rows="4"
                required
              ></textarea>
            </div>

            <button type="submit" class="btn-submit">Kirim</button>
          </form>
        </div>
      </div>
    </main>

    <footer class="footer">
      <p>© 2026 SMK Yadika Soreang - Onlineshop Sekolah</p>
    </footer>
  </div>
</template>

<script setup>
import { ref } from "vue";

const formData = ref({
  name: "",
  email: "",
  message: "",
});

const handleSubmit = () => {
  alert(`Pesan dari ${formData.value.name} telah dikirim!`);
  formData.value = {
    name: "",
    email: "",
    message: "",
  };
};
</script>

<style scoped>
.contact-page {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  color: #5a4b51;
  background-color: #fff9fa;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 3rem;
  background-color: #ffffff;
  box-shadow: 0 2px 10px rgba(230, 180, 195, 0.15);
}

.brand {
  font-weight: bold;
  font-size: 1.1rem;
  color: #d87093;
}

.nav-links {
  display: flex;
  gap: 1.5rem;
}

.nav-links a {
  text-decoration: none;
  color: #8c717a;
  font-size: 0.95rem;
  transition: color 0.3s;
}

.nav-links a:hover,
.nav-links a.active {
  color: #d87093;
  font-weight: 600;
  border-bottom: 2px solid #d87093;
  padding-bottom: 2px;
}

.hero-banner {
  background-color: #f8c8d8; /* Soft pink dominan */
  color: #6b3e4e;
  text-align: center;
  padding: 2.5rem 1rem;
}

.hero-banner h1 {
  margin: 0;
  font-size: 1.8rem;
  font-weight: 600;
  letter-spacing: 0.5px;
}

.content-container {
  max-width: 900px;
  width: 100%;
  margin: 2.5rem auto;
  padding: 0 1.5rem;
  flex: 1;
}

.contact-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 3rem;
}

.contact-info h2,
.contact-form-section h2 {
  font-size: 1.3rem;
  margin-bottom: 1.5rem;
  color: #4a383f;
}

.info-item {
  margin-bottom: 1.2rem;
}

.info-header {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  color: #c95b83;
}

.info-header .icon {
  font-size: 1.1rem;
}

.info-item p {
  margin: 0.2rem 0 0 1.6rem;
  font-size: 0.9rem;
  color: #735d65;
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.form-group {
  display: flex;
  flex-direction: column;
  gap: 0.3rem;
}

.form-group label {
  font-size: 0.85rem;
  color: #5a4b51;
  font-weight: 500;
}

.form-group input,
.form-group textarea {
  padding: 0.6rem 0.8rem;
  border: 1px solid #f1c6d3;
  border-radius: 6px;
  background-color: #fff;
  font-size: 0.9rem;
  color: #4a383f;
  outline: none;
  transition: border-color 0.3s;
}

.form-group input:focus,
.form-group textarea:focus {
  border-color: #d87093;
  box-shadow: 0 0 0 3px rgba(216, 112, 147, 0.15);
}

.form-group input::placeholder,
.form-group textarea::placeholder {
  color: #c7b2b8;
}

.btn-submit {
  align-self: flex-start;
  background-color: #d87093; /* Soft Pink / Rose Button */
  color: white;
  border: none;
  padding: 0.5rem 1.8rem;
  border-radius: 20px; /* Bentuk rounded oval sesuai sampel */
  font-size: 0.9rem;
  cursor: pointer;
  transition:
    background-color 0.3s,
    transform 0.1s;
  margin-top: 0.5rem;
}

.btn-submit:hover {
  background-color: #c55c80;
}

.btn-submit:active {
  transform: scale(0.98);
}

.footer {
  text-align: center;
  padding: 1.5rem;
  font-size: 0.8rem;
  color: #a38d94;
  border-top: 1px solid #fae3eb;
}

@media (max-width: 768px) {
  .contact-grid {
    grid-template-columns: 1fr;
    gap: 2rem;
  }

  .navbar {
    flex-direction: column;
    gap: 0.8rem;
    padding: 1rem;
  }
}
</style>
