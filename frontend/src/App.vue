<template>
  <div class="text-white min-vh-100 py-5">
    <!-- Hero -->
    <section class="py-5 text-center hero-gradient">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-md-6 mb-4 mb-md-0">
            <img src="./assets/menu_cireng.jpg" alt="Cireng RR" class="img-fluid rounded shadow" />
          </div>
          <div class="col-md-6">
            <h2 class="text-warning mb-3">Kenapa Pilih Cireng RR?</h2>
            <ul class="list-unstyled text-secondary fs-5 text-start">
              <li>✅ Tekstur renyah di luar, lembut di dalam</li>
              <li>✅ Bumbu racikan khas RR</li>
              <li>✅ Cocok untuk semua suasana</li>
              <li>✅ Halal & fresh dibuat setiap hari</li>
            </ul>
            <a :href="whatsappUrl" target="_blank" class="btn btn-warning mt-3 fw-semibold">
              Pesan Sekarang via WhatsApp
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- Varian Rasa -->
    <section class="py-5 bg-black">
      <div class="container text-center">
        <h2 class="mb-4 text-warning">Varian Rasa</h2>
        <div class="row g-4">
          <div class="col-md-4">
            <div class="card text-light border-warning">
              <img :src="smoked_beef" class="card-img-top" alt="smoked_beef" />
              <div class="card-body">
                <h5 class="card-title">Smoked Beef</h5>
                <p class="card-text">Gurih & klasik. Nice choice!</p>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card text-light border-warning">
              <img :src="mozzarella" class="card-img-top" alt="mozzarella" />
              <div class="card-body">
                <h5 class="card-title">Mozzarella</h5>
                <p class="card-text">Lelehan keju di setiap gigitan!</p>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card text-light border-warning">
              <img :src="sosis" class="card-img-top" alt="sosis" />
              <div class="card-body">
                <h5 class="card-title">Sosis</h5>
                <p class="card-text">Potongan sosis yang bikin nagih!</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Tentang -->
    <section class="py-5 bg-dark">
      <div class="container text-center">
        <h2 class="mb-4 text-warning">Tentang Cireng RR</h2>
        <p class="lead">
          Kami adalah UMKM lokal yang menyediakan camilan cireng dengan berbagai rasa unik dan kualitas
          terbaik. Dibuat dengan cinta dan resep turun-temurun.
        </p>
      </div>
    </section>

    <!-- Footer / Kontak -->
    <footer class="py-4 bg-black text-center text-light border-top border-warning">
      <div class="container">
        <div class="mb-2">
          <i class="bi bi-geo-alt-fill text-warning me-2"></i> DKI Jakarta, Jakarta Timur
        </div>
        <div class="mb-2">
          <i class="bi bi-whatsapp text-success me-2"></i>
          <a :href="whatsappUrl" target="_blank" class="text-decoration-none text-light">+62 896-9321-8083</a>
        </div>
        <div class="mb-3">
          <i class="bi bi-envelope-fill text-warning me-2"></i> cirengrr@gmail.com
        </div>
        <div class="d-flex justify-content-center gap-3">
          <a href="#" class="text-warning"><i class="bi bi-instagram fs-4"></i></a>
          <a href="#" class="text-warning"><i class="bi bi-tiktok fs-4"></i></a>
        </div>
        <p class="mb-2">© 2025 Cireng RR. All rights reserved.</p>
      </div>
    </footer>
  </div>
</template>

<script lang="ts" setup>
import smoked_beef from './assets/cireng1.jpg'
import mozzarella from './assets/cireng1.jpg'
import sosis from './assets/cireng1.jpg'

// Ganti nomor WhatsApp di sini
const phoneNumber = '6289693218083'
const message = 'Halo Cireng RR! Saya mau pesan cirengnya dong'
const whatsappUrl = `https://wa.me/${phoneNumber}?text=${encodeURIComponent(message)}`
</script>

<style scoped>
.hero-gradient {
  background: linear-gradient(135deg, #111 0%, #222 100%);
}

.card-img-top {
  height: 200px;
  object-fit: cover;
}
</style>
