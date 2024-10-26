# 🌐 Wiki Dokumentasi: Dashboard & Web App Berbasis Z-Score WHO dengan Heat Map dan Sistem Prediktif AI untuk Pemantauan Stunting Balita 🌐

## 📖 Pengantar

Stunting atau gagal tumbuh adalah masalah kesehatan yang signifikan, terutama di negara-negara berkembang. Untuk memantau dan mengatasi risiko ini, teknologi digital berbasis data memberikan solusi yang dapat diandalkan. Dengan menggunakan _Dashboard & Web App_ berbasis analisis Z-Score WHO, sistem ini memungkinkan pemantauan kesehatan balita berdasarkan parameter seperti tinggi, berat, lingkar kepala, dan status ASI eksklusif. Sistem ini dirancang dengan fitur Heat Map Regional, Z-Score Analytics, dan Sistem Prediktif AI untuk memantau, menganalisis, dan mengintervensi kondisi stunting secara tepat.

## 🔍 Komponen Utama Sistem

1. Heat Map Regional  
   Heat Map ini menampilkan data secara geografis, membantu tenaga kesehatan dan pemerintah daerah memantau wilayah dengan risiko tinggi stunting. Berdasarkan data yang dikumpulkan, sistem ini mengelompokkan area ke dalam zona risiko yang berbeda untuk mempermudah pengalokasian sumber daya secara efektif.

2. Z-Score Analytics  
   Berdasarkan Z-Score WHO, sistem mengkategorikan kesehatan balita dalam parameter tinggi-badan dan berat-badan menurut umur, serta lingkar kepala. Analisis ini membantu dalam menilai status kesehatan balita secara individual maupun regional.

3. Sistem Prediktif AI  
   Menggunakan algoritma pembelajaran mesin, sistem ini dapat memprediksi balita yang berisiko mengalami stunting di masa depan, memberikan intervensi dini untuk mencegah kondisi tersebut.

## 🧠 Bagian 1: Heat Map Regional - Menyediakan Visualisasi Risiko Stunting yang Efektif 🧠

Heat Map Regional merupakan fitur utama yang dirancang untuk memantau penyebaran risiko stunting dalam skala geografis. Dengan data yang di-update secara berkala, fitur ini menjadi alat yang krusial dalam pemantauan kesehatan masyarakat.

### 1. Teknologi dan Algoritma Pembuatan Heat Map

- Sumber Data. Sistem mengumpulkan data dari berbagai pusat kesehatan dan entitas pemerintahan yang telah memiliki catatan Z-Score berdasarkan WHO. Data ini meliputi lokasi geografis, umur, berat, tinggi badan, lingkar kepala, serta status ASI eksklusif.

- Algoritma Pengelompokan Data. Dengan algoritma _Clustering_, data disegmentasikan berdasarkan tingkat risiko, seperti _Normal_, _Berisiko_, dan _Stunting_. Teknik _K-Means Clustering_ sering digunakan untuk menentukan kelompok risiko berdasarkan parameter kesehatan balita.

- Teknologi Heat Map. Visualisasi ini memanfaatkan teknologi _GIS (Geographic Information System)_ dan _Leaflet_ atau _Mapbox_ untuk menampilkan data pada peta interaktif. Dengan demikian, pengguna dapat memantau zona risiko dan mengambil tindakan tepat waktu.

### 2. Manfaat Heat Map bagi Pemerintah dan Tenaga Kesehatan

- Alokasi Sumber Daya yang Tepat Sasaran. Dengan informasi risiko pada level geografis, pemerintah daerah dapat mengarahkan lebih banyak sumber daya ke daerah dengan prevalensi stunting yang tinggi.

- Intervensi Kesehatan yang Terukur. Heat Map membantu tenaga kesehatan menetapkan prioritas intervensi yang berdasarkan data faktual, sehingga tindakan seperti penyuluhan gizi atau pembagian suplemen lebih efisien.

### 3. Contoh Tampilan Heat Map dan Penggunaan Warna Risiko

| Warna Risiko | Tingkat Risiko         |
| ------------ | ---------------------- |
| 🔴 Merah     | Risiko Stunting Tinggi |
| 🟠 Oranye    | Risiko Sedang          |
| 🟢 Hijau     | Risiko Rendah          |

_Gambar di bawah ini memperlihatkan contoh heat map interaktif yang menampilkan area dengan tingkat risiko stunting yang bervariasi._

![Contoh Heat Map Risiko Stunting](https://example.com/heatmap_risiko_stunting.png)

## 📊 Bagian 2: Z-Score Analytics - Analisis Kesehatan Balita Berdasarkan Z-Score WHO 📊

Analisis berbasis Z-Score WHO menjadi komponen kunci dalam pemantauan kesehatan balita. Sistem ini menggunakan parameter tinggi, berat, lingkar kepala, dan status ASI eksklusif untuk memberikan gambaran lengkap mengenai kondisi kesehatan balita.

### 1. Dasar Z-Score WHO dan Pengukurannya

- Parameter Utama Z-Score. WHO mengembangkan sistem Z-Score untuk memetakan pertumbuhan normal balita. Z-Score mengukur standar deviasi data anak dari nilai rata-rata populasi, mengelompokkan mereka ke dalam kategori seperti _Normal_, _Moderate_, atau _Severe Stunting_.

- Kategori Z-Score dan Deskripsi.

  - Tinggi-Badan per Umur (HAZ). Mengukur tinggi balita dibandingkan rata-rata usia.
  - Berat-Badan per Umur (WAZ). Mengukur berat balita berdasarkan usia.
  - Lingkar Kepala. Membantu memantau perkembangan otak dan kondisi kesehatan lain yang berhubungan dengan pertumbuhan.
  - Status ASI Eksklusif. Data ini digunakan sebagai variabel tambahan untuk menilai gizi optimal balita, karena ASI eksklusif berhubungan erat dengan kesehatan dan perkembangan balita.

### 2. Implementasi dan Pengolahan Data Z-Score dalam Dashboard

Sistem ini secara otomatis menghitung Z-Score balita berdasarkan input dari tenaga kesehatan. Data ini kemudian dipetakan dalam tampilan dashboard yang menampilkan perkembangan balita per daerah, dengan warna dan indikator yang menandakan tingkat risiko.

- Visualisasi Dashboard. Dashboard menampilkan grafik perkembangan kesehatan yang mencakup berat, tinggi, lingkar kepala, dan status ASI. Dengan bantuan grafik dan diagram batang, pengguna dapat memantau perubahan yang terjadi pada balita secara mudah.

- Tabel Z-Score WHO pada Dashboard

  | Kategori Z-Score   | Status Risiko | Warna Indikator |
  | ------------------ | ------------- | --------------- |
  | >= -1 SD           | Normal        | 🟢 Hijau        |
  | -2 SD sampai -1 SD | Risiko Sedang | 🟠 Oranye       |
  | < -2 SD            | Stunting      | 🔴 Merah        |

- Contoh Tampilan Z-Score  
  Gambar berikut menunjukkan contoh tampilan Z-Score pada dashboard yang menunjukkan status kesehatan setiap balita berdasarkan parameter WHO:

  ![Contoh Tampilan Z-Score Dashboard](https://example.com/zscore_dashboard.png)

### 3. Manfaat Z-Score Analytics dalam Pemantauan Kesehatan Balita

- Evaluasi Kesehatan Secara Real-Time. Dashboard ini membantu tenaga kesehatan untuk mengevaluasi status kesehatan balita secara cepat dan akurat.

- Akurasi dalam Pengambilan Keputusan. Dengan pemetaan skor risiko, tenaga kesehatan bisa menentukan langkah-langkah lanjutan berdasarkan data yang akurat, termasuk pemeriksaan tambahan atau intervensi gizi.

## 🔮 Bagian 3: Sistem Prediktif AI untuk Deteksi Dini Risiko Stunting 🔮

Dengan memanfaatkan Artificial Intelligence (AI), sistem ini dapat melakukan analisis prediktif untuk mendeteksi risiko stunting di masa depan. Hal ini memungkinkan intervensi gizi dan kesehatan sebelum balita menunjukkan gejala stunting.

### 1. Teknologi dan Algoritma yang Digunakan dalam Sistem Prediktif AI

- Penggunaan Pembelajaran Mesin (Machine Learning). Algoritma _Random Forest_ dan _Support Vector Machine (SVM)_ digunakan untuk menganalisis data perkembangan kesehatan dari waktu ke waktu. Model ini dilatih dengan data riwayat kesehatan untuk memprediksi kemungkinan stunting berdasarkan pola pertumbuhan.

- Proses Pelatihan Model AI. Model dilatih menggunakan data historis balita dari berbagai daerah, yang mencakup tinggi, berat, lingkar kepala, dan status ASI eksklusif. Dengan data ini, AI dapat mengidentifikasi pola-pola risiko stunting yang mungkin terjadi.

- Teknologi Prediksi Berbasis Grafik Pertumbuhan. Data Z-Score sebelumnya digunakan untuk menciptakan grafik prediktif yang menunjukkan potensi perkembangan balita. Grafik ini membantu menunjukkan potensi risiko jika tren pertumbuhan tidak membaik.

### 2. Penerapan AI dalam Pemantauan Kesehatan Balita

- Prediksi dan Peringatan Dini. Sistem memberikan peringatan jika suatu pola perkembangan mengindikasikan risiko stunting. Peringatan ini memungkinkan orang tua dan tenaga kesehatan untuk memberikan perhatian lebih pada balita tersebut.

- Evaluasi Intervensi Gizi. Berdasarkan prediksi AI, orang tua atau tenaga kesehatan dapat mengambil langkah-langkah seperti pemberian suplemen atau konseling gizi.

- Dukungan Keputusan Berbasis Data. Hasil prediksi AI ditampilkan pada dashboard dalam bentuk visualisasi sederhana, seperti grafik yang menunjukkan kemungkinan perkembangan atau risiko berdasarkan data pertumbuhan sebelumnya.

### 3. Tabel: Contoh Algoritma dan Parameter yang Digunakan dalam Prediksi AI

| Algoritma AI | Deskripsi Singkat |

| Parameter Utama |
| --------------- | ------------------------------------------ | ----------------------------------------- |
| Random Forest   | Algoritma _ensemble_ untuk prediksi risiko | Tinggi, berat, lingkar kepala, status ASI |
| SVM             | Memetakan risiko berdasarkan margin besar  | Pertumbuhan tinggi dan berat              |
| Neural Network  | Model kompleks untuk pola pertumbuhan      | Z-Score WHO dan pola pertumbuhan          |

## 📈 Bagian 4: Manfaat Bisnis dan Pengguna

### 1. Efisiensi Pengambilan Keputusan di Tingkat Pemerintah Daerah

Dashboard ini memberikan akses data secara langsung bagi pemerintah daerah untuk memahami dan mengelola prevalensi stunting di wilayahnya. Ini mempermudah alokasi sumber daya dan menetapkan prioritas intervensi kesehatan yang tepat.

### 2. Dukungan bagi Tenaga Kesehatan

Dengan visualisasi data kesehatan balita yang lengkap, tenaga kesehatan dapat segera mengetahui status kesehatan pasien dan menentukan tindakan selanjutnya dengan mudah. Informasi yang real-time membantu pengambilan keputusan yang lebih baik dan intervensi lebih awal.

### 3. Akses Informasi bagi Orang Tua

Aplikasi berbasis web ini bisa diakses oleh orang tua, memberikan mereka akses terhadap perkembangan kesehatan anak secara langsung. Melalui notifikasi dan peringatan, orang tua bisa mengambil langkah-langkah preventif untuk memastikan kesehatan optimal bagi anak.

## 📷 Gambar Pendukung dan Diagram

1. Diagram Alur Sistem Dashboard & Web App  
   Diagram ini menampilkan alur data dari input balita hingga visualisasi di dashboard dan analisis prediktif.

   ![Diagram Alur Dashboard Stunting](https://example.com/diagram_dashboard.png)

2. Contoh Grafik Prediksi AI  
   Gambar ini menunjukkan grafik prediksi yang memperlihatkan kemungkinan tren pertumbuhan balita.

   ![Contoh Grafik Prediksi AI](https://example.com/grafik_prediksi_ai.png)

## 🎯 Kesimpulan dan Rekomendasi

Dashboard & Web App Berbasis Z-Score WHO dengan Heat Map dan AI ini menawarkan solusi menyeluruh dalam pemantauan kesehatan balita, khususnya dalam upaya penanggulangan stunting. Dengan teknologi visualisasi, analisis berbasis data, dan prediksi AI, sistem ini mampu memberikan panduan bagi pemerintah, tenaga kesehatan, dan orang tua dalam mendeteksi risiko stunting sedini mungkin.
