<template>
  <section class="landing-page">
    <h1>Selamat Datang di Onlineshop Sekolah</h1>
    <p>Belanja gampang, sekolah senang.</p>
    <button class="btn-grad" type="button">produk kami</button>
  </section>

  <section class="feature-grid">
    <article class="feature-card">
      <h2>kualitas terjamin</h2>
      <p>bahan berkualitas!!</p>
    </article>
    <article class="feature-card">
      <h2>kualitas terjamin</h2>
      <p>bahan berkualitas!!</p>
    </article>
    <article class="feature-card">
      <h2>kualitas terjamin</h2>
      <p>bahan berkualitas!!</p>
    </article>
  </section>

  <main>
    <h1 class="h1">Kelinci Gendut</h1>
    <video controls width="480" muted loop>
      <source src="/video/mov_bbb (1).mp4" type="video/mp4" />
      Browser kamu tidak mendukung pemutaran video.
    </video>
  </main>
</template>

<style scoped>
.h1 {
  text-align: center;
  color: #2c3e50;
  margin-top: 2rem;
}
video {
  margin: 0 auto;
  margin-top: 16px;
  border-radius: 10px;
  display: block;
}

.landing-page {
  text-align: center;
  padding: 2.5rem 1.5rem;
  margin-top: 1.5rem;
  background: linear-gradient(135deg, #ffc0cb, #ffe5ea);
  border-radius: 16px;
  box-shadow:
    0 18px 36px rgba(255, 110, 127, 0.24),
    0 10px 22px rgba(0, 0, 0, 0.12),
    0 2px 6px rgba(0, 0, 0, 0.08);
}

.landing-page h1 {
  font-size: clamp(2rem, 3vw, 2.7rem);
  color: #2c3e50;
}

.landing-page p {
  margin-top: 10px;
  color: #4d5360;
  font-size: 1rem;
}

.feature-grid {
  display: flex;
  gap: 24px;
  flex-wrap: wrap;
  justify-content: center;
  margin: 2rem 0 2.5rem;
}

.feature-card {
  flex: 1 1 240px;
  max-width: 320px;
  padding: 32px 24px;
  background: linear-gradient(135deg, #ffe5ea, #ffc0cb);
  border-radius: 16px;
  box-shadow:
    0 18px 36px rgba(255, 110, 127, 0.24),
    0 10px 22px rgba(0, 0, 0, 0.12),
    0 2px 6px rgba(0, 0, 0, 0.08);
  text-align: center;
  transition:
    transform 0.3s ease,
    box-shadow 0.3s ease;
}

.feature-card h2 {
  font-size: 1.2rem;
  color: #2c3e50;
}

.feature-card p {
  margin-top: 6px;
  color: #4d5360;
}

.btn-grad {
  margin-top: 1.2rem;
  padding: 15px 30px;
  border: none;
  border-radius: 10px;
  background-image: linear-gradient(
    to right,
    #ff6e7f 0%,
    #bfe9ff 51%,
    #ff6e7f 100%
  );
  background-size: 200% auto;
  color: #fff;
  text-transform: uppercase;
  font-weight: 700;
  letter-spacing: 0.04em;
  box-shadow: 0 8px 18px rgba(255, 110, 127, 0.22);
  cursor: pointer;
}

.btn-grad:hover {
  background-position: right center;
}

@media (max-width: 768px) {
  .feature-grid {
    grid-template-columns: 1fr;
  }
}
</style>
