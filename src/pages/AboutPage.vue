<template>
  <div class="about-container">
    <section class="hero-banner">
      <h1>about us</h1>
    </section>

    <section class="section-story">
      <div class="story-content">
        <h2>our story</h2>
        <p>
          Onlineshop ini dikelola langsung oleh siswa SMK Yadika Soreang jurusan
          PPLG yang bernama renatta cantik, sebagai proyek belajar sekaligus
          membantu teman-teman mendapatkan perlengkapan sekolah dengan mudah dan
          harga terjangkau.
        </p>
        <p>
          Setiap produk dipilih dan dikurasi oleh tim kecil siswa, dengan
          pengambilan langsung di koperasi sekolah.
        </p>
      </div>
      <div class="toko.jpg">
        <img src="/toko.jpg" alt="Toko" class="story-image-placeholder" />
      </div>
    </section>

    <section class="section-team">
      <h2 class="team-title">the team</h2>
      <div class="team-cards">
        <div class="team-card">
          <div class="avatar"><img src="/renattaaa.jpg" alt="Renattaaa" /></div>
          <h3>renatta</h3>
          <p>team lead</p>
        </div>

        <div class="team-card">
          <div class="avatar"><img src="/kaisa.jpg" alt="Kaisa" /></div>
          <h3>kaisa</h3>
          <p>developer</p>
        </div>

        <div class="team-card">
          <div class="avatar"><img src="/nasyo.jpg" alt="Nasyandra" /></div>
          <h3>nasyandra</h3>
          <p>Desain & UI</p>
        </div>
      </div>
    </section>

    <footer class="footer">
      <p>© 2026 SMK Yadika Soreang - Onlineshop Sekolah</p>
    </footer>
  </div>
</template>

<style scoped>
.about-container {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  color: #333;
  background-color: #fff5f7;
  min-height: 100vh;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 50px;
  background-color: #ffffff;
  border-bottom: 1px solid #fce4ec;
}

.logo {
  font-weight: bold;
  color: #ff98b0;
  font-size: 1.1rem;
}

.nav-links a {
  margin-left: 20px;
  text-decoration: none;
  color: #666;
  font-size: 0.95rem;
}

.nav-links a.active {
  color: #fcc0d6;
  font-weight: bold;
  border-bottom: 2px solid #f6abc6;
  padding-bottom: 4px;
}

/* 2. Hero Banner */
.hero-banner {
  background-color: #ffb0cd;
  color: white;
  text-align: center;
  padding: 40px 20px;
  margin: 20px 60px;
  border-radius: 4px;
}

.hero-banner h1 {
  margin: 0;
  font-size: 2rem;
  font-weight: 600;
}

/* 3. Section Cerita Kami */
.section-story {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 40px 80px;
  gap: 40px;
}

.story-content {
  flex: 1;
}

.story-content h2 {
  color: #880e4f;
  margin-bottom: 15px;
}

.story-content p {
  color: #555;
  line-height: 1.6;
  font-size: 0.95rem;
  margin-bottom: 12px;
}

.story-image-placeholder {
  flex: 1;
  height: 200px;
  background-color: #f8bbd0; /* Soft Light Pink */
  border-radius: 12px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #880e4f;
  font-weight: 500;
  border: 1px dashed #c2185b;
}

/* 4. Section Tim Kami */
.section-team {
  background-color: #fce4ec; /* Background area tim yang sedikit berbeda */
  padding: 40px 80px 60px 80px;
  margin: 20px 60px;
  border-radius: 12px;
  text-align: center;
}

.team-title {
  color: #880e4f;
  margin-bottom: 30px;
}

.team-cards {
  display: flex;
  justify-content: center;
  gap: 30px;
}

.team-card {
  background-color: #ffffff;
  padding: 25px 35px;
  border-radius: 16px;
  box-shadow: 0 4px 12px rgba(216, 27, 96, 0.08);
  display: flex;
  flex-direction: column;
  align-items: center;
  min-width: 140px;
}

.avatar {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background-color: #e91e63; /* Pink Vivid */
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 15px;
}

.team-card h3 {
  margin: 5px 0 2px 0;
  font-size: 1.1rem;
  color: #333;
}

.team-card p {
  margin: 0;
  font-size: 0.85rem;
  color: #777;
}

/* 5. Footer */
.footer {
  text-align: center;
  padding: 20px;
  color: #a34e6e;
  font-size: 0.85rem;
  margin-top: 40px;
}
</style>
