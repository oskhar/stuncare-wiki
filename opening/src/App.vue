<!-- App.vue -->
<template>
  <v-app>
    <v-main class="white-background">
      <!-- Hero Section -->
      <v-container class="text-center">
        <v-row justify="center" align="center">
          <v-col cols="12" md="8">
            <!-- Logo -->
            <center>
              <v-img
                src="logo.png"
                alt="Stuncare Logo"
                max-width="200"
                class="logo-app mb-10 mt-5"
              ></v-img>
            </center>

            <!-- Title and Subtitle -->
            <h1 class="display-3 font-weight-bold title-text mb-4">Stuncare - Knowladge Base</h1>
            <p class="font-weight-medium subtitle-text mb-6">
              Solusi Komprehensif untuk Menurunkan Tingkat Stunting di Indonesia
            </p>

            <!-- Action Buttons -->
            <v-btn
              color="primary"
              class="mb-4 btn-main px-5"
              large
              href="https://github.com/oskhar/stuncare-wiki/blob/main/README.md"
            >
              Mulai Sekarang
            </v-btn>

            <!-- Introduction Text -->
            <p class="intro-text mb-16">
              Kami hadir untuk mendukung masa depan sehat generasi Indonesia melalui teknologi yang mengintegrasikan pemantauan, analisis, dan intervensi kesehatan yang akurat.
            </p>
          </v-col>
        </v-row>
      </v-container>

      <!-- Features Section -->
      <v-container class="text-center pt-8">
        <v-row justify="center">
          <v-col cols="12" md="10">
            <v-divider class="my-6"></v-divider>
            <v-row>
              <v-col
                v-for="(item, index) in features"
                :key="index"
                cols="12"
                sm="6"
                md="4"
                class="mb-4 feature-item"
              >
                <h3 class="font-weight-medium feature-title mb-2">
                  {{ item.title }}
                </h3>
                <p class="feature-description">
                  {{ item.description }}
                </p>
              </v-col>
            </v-row>
            <v-divider class="my-6"></v-divider>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",
  data() {
    return {features: [
  { 
    title: "Smart IoT Monitoring", 
    description: "Sistem IoT untuk pemantauan berat dan tinggi balita secara otomatis dan real-time." 
  },
  { 
    title: "Dashboard Z-Score WHO", 
    description: "Analisis risiko stunting melalui heat map dan prediksi AI berbasis Z-Score WHO." 
  },
  { 
    title: "AI-based Intervensi & Edukasi", 
    description: "Rekomendasi nutrisi real-time dan edukasi interaktif untuk orang tua." 
  },
  { 
    title: "Evaluasi & Feedback", 
    description: "Laporan berkala dan feedback dari orang tua untuk efektivitas intervensi." 
  },
  { 
    title: "Ekspansi & Dampak", 
    description: "Memperluas cakupan layanan untuk meningkatkan penanganan stunting." 
  },
  { 
    title: "Dokumentasi Teknis", 
    description: "Panduan lengkap untuk memahami teknologi dan infrastruktur kami." 
  },
],

    };
  },
};
</script>

<style scoped>
body {
  background-color: #eff8fc !important;
}

.white-background {
  background-color: #fff !important;
}

.logo-app {
  border-radius: 20px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Memberikan efek bayangan lembut */
}

.title-text {
  color: #2b6e6e; /* Warna yang sesuai dengan logo */
  font-size: 3rem;
}

.subtitle-text {
  color: #4a4a4a;
  font-size: 1.25rem;
}

.btn-main {
  background-color: #447f8e !important; /* Warna tombol utama sesuai logo */
  color: #fff !important;
  height: 100px; /* Atur tinggi tombol */
  font-size: 1.1rem; /* Ukuran font tombol */
  padding: 0 50px; /* Padding untuk tombol */
  font-weight: bold;
}

.btn-outline {
  color: #2b6e6e !important;
  border-color: #2b6e6e !important;
}

.intro-text {
  color: #6c757d;
  font-size: 1rem;
}

.feature-item {
  padding: 1rem;
}

.feature-title {
  color: #2b6e6e;
  font-weight: 700;
}

.feature-description {
  color: #6c757d;
}
.content-center {
  text-align: center;
}
</style>
