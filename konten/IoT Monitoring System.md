[**<<< Kembali**](../README.md)

# 🌐 Sistem Pemantauan Pintar untuk Tinggi dan Lingkar Kepala Balita 🌐

## 📖 Pengantar

Sistem pemantauan kesehatan balita yang terotomatisasi merupakan terobosan dalam teknologi kesehatan. Dengan memanfaatkan _Computer Vision_ dan _Internet of Things_ (IoT), sistem ini membantu memantau perkembangan balita secara akurat, cepat, dan terintegrasi dengan cloud. Dokumen ini akan memandu Anda melalui dua jalur implementasi utama: _Computer Vision_ sebagai jalur utama dan _Smart Scale IoT_ sebagai alternatif, keduanya dirancang untuk memenuhi kebutuhan pemantauan kesehatan anak yang akurat, aman, dan mudah digunakan.

## 🔍 Ringkasan Jalur Implementasi

1. Jalur Utama. Computer Vision  
   Menggunakan teknologi _Computer Vision_ yang dapat mengukur tinggi dan lingkar kepala balita melalui kamera tanpa kontak fisik. Jalur ini mengutamakan fleksibilitas, skalabilitas, dan biaya yang lebih terjangkau dibandingkan sensor fisik.

2. Jalur Alternatif. Smart Scale IoT  
   Menggunakan perangkat sensor fisik yang terhubung melalui IoT untuk mengukur tinggi, berat, dan parameter kesehatan lainnya. Jalur ini lebih tepat untuk penggunaan yang membutuhkan akurasi langsung dengan alat khusus di lingkungan klinis.

## ⚙️ Bagian 1: Jalur Utama - Computer Vision untuk Pengukuran Tinggi dan Lingkar Kepala

##### 📏 Deskripsi Teknologi Computer Vision dalam Pengukuran Kesehatan

_Computer Vision_ merupakan teknologi berbasis pengolahan gambar yang mampu mengidentifikasi, melacak, dan mengukur objek secara otomatis. Dalam konteks pemantauan kesehatan balita, _Computer Vision_ memanfaatkan algoritma yang memproses data visual dari kamera untuk mengukur tinggi dan lingkar kepala dengan akurasi tinggi.

##### 1. Teknologi dan Algoritma Utama yang Digunakan

- Pengenalan dan Pelacakan Titik Tubuh  
  Teknologi seperti _OpenPose_ atau _MediaPipe_ memungkinkan pengenalan titik-titik tubuh (misalnya, kepala, bahu, dan dagu) yang dapat digunakan untuk pengukuran tinggi. Dengan pelacakan real-time, sistem dapat menghitung tinggi badan berdasarkan perbandingan dengan objek referensi yang diketahui.

- Pengukuran Proporsi untuk Estimasi Lingkar Kepala  
  Algoritma _Contour Detection_ dan _Edge Detection_ digunakan untuk mendeteksi dan memetakan lingkar kepala balita. Metode ini menggunakan titik referensi pada wajah (seperti jarak mata atau dahi) untuk menghitung diameter dan lingkar kepala dengan akurasi yang baik.

- Kalibrasi Berbasis Ruang dan Skala  
  Sebelum pengukuran, ruang harus dikalibrasi untuk mendapatkan referensi skala. Hal ini bisa dilakukan dengan objek standar yang ukurannya diketahui (misalnya, penggaris) di dalam area gambar.

##### 2. Proses Implementasi Computer Vision dalam Pengukuran Tinggi dan Lingkar Kepala

- Tahap 1: Pengambilan Gambar atau Video Balita  
  Kamera yang terhubung ke sistem akan menangkap gambar atau video balita. Pengambilan gambar ini dapat dilakukan di rumah atau pusat kesehatan dengan posisi tubuh balita yang tepat.

- Tahap 2: Deteksi Titik Tubuh dan Wajah  
  Sistem _Computer Vision_ akan mengenali titik tubuh yang relevan, seperti bagian atas kepala, dagu, bahu, dan titik di sekitar kepala untuk estimasi lingkar. Teknologi ini mengutamakan keamanan dan kenyamanan, karena hanya membutuhkan pencahayaan yang memadai.

- Tahap 3: Pengukuran dan Konversi Skala  
  Berdasarkan titik-titik yang telah dikenali, sistem menghitung tinggi dan lingkar kepala. Pengukuran ini dikonversi ke unit metrik sebenarnya (misalnya, cm) menggunakan skala dari kalibrasi awal.

- Tahap 4: Penyimpanan dan Pengolahan Data  
  Data yang telah diukur langsung disimpan di cloud dan dapat diakses melalui aplikasi untuk pemantauan dan analisis kesehatan balita.

##### 3. Keuntungan Utama Jalur Computer Vision

- Tanpa Kontak Fisik. Menghilangkan kebutuhan perangkat yang menyentuh balita, sehingga lebih nyaman dan higienis.
- Biaya Lebih Rendah. Hanya membutuhkan kamera standar dan aplikasi, mengurangi investasi pada perangkat fisik tambahan.
- Fleksibilitas dan Skalabilitas. Mudah diterapkan di berbagai lingkungan, seperti di rumah atau klinik.

## 🔄 Bagian 2: Jalur Alternatif - Smart Scale IoT untuk Pengukuran Berat, Tinggi, dan Data Kesehatan Lainnya

##### 📏 Deskripsi Teknologi Smart Scale IoT

_Smart Scale IoT_ adalah perangkat terhubung dengan sensor yang tidak hanya mengukur berat, tetapi juga tinggi, dan dapat dilengkapi dengan sensor tambahan untuk parameter kesehatan lain, seperti suhu tubuh dan kadar hemoglobin. Data dari alat ini terhubung langsung ke cloud, sehingga dapat diakses dan dipantau oleh tenaga kesehatan.

##### 1. Teknologi dan Komponen Utama Smart Scale IoT

- Sensor Berat dan Tinggi Badan  
  Sensor strain gauge digunakan untuk mengukur berat badan dengan presisi tinggi, sedangkan sensor ultrasonik atau inframerah digunakan untuk tinggi badan. Data ini langsung ditransfer ke aplikasi melalui konektivitas IoT.

- Sensor Suhu dan Kadar Hemoglobin  
  Alat ini bisa dilengkapi dengan sensor tambahan seperti termokopel untuk suhu dan painless lancet untuk pengukuran hemoglobin melalui darah kapiler. Sensor tambahan ini memberikan data penting untuk deteksi dini kondisi kesehatan seperti anemia.

##### 2. Proses Implementasi Smart Scale IoT

- Tahap 1: Penimbangan dan Pengukuran Tinggi Badan  
  Balita ditempatkan pada alat timbang yang terhubung, yang kemudian melakukan pengukuran berat dan tinggi secara otomatis.

- Tahap 2: Pengukuran Suhu dan Kadar Hemoglobin (Opsional)  
  Jika alat dilengkapi dengan sensor tambahan, suhu tubuh dan kadar hemoglobin juga dapat diukur dalam waktu yang singkat.

- Tahap 3: Transfer dan Sinkronisasi Data  
  Data langsung ditransfer ke cloud menggunakan protokol MQTT atau BLE (Bluetooth Low Energy), yang memungkinkan pemantauan data secara real-time.

##### 3. Keuntungan dan Keterbatasan Jalur Smart Scale IoT

- Keunggulan. Menghasilkan data yang sangat akurat untuk pengukuran berat dan tinggi, lebih cocok untuk lingkungan klinis dengan standar akurasi tinggi.
- Keterbatasan. Memerlukan kontak fisik dan perangkat tambahan, sehingga membutuhkan biaya investasi lebih tinggi.

## 📊 Tabel Perbandingan Jalur Computer Vision vs Smart Scale IoT

| Fitur                  | Jalur Computer Vision                        | Jalur Smart Scale IoT                   |
| ---------------------- | -------------------------------------------- | --------------------------------------- |
| Akurasi Tinggi Badan   | Menggunakan skala referensi visual           | Sensor fisik (lebih akurat)             |
| Akurasi Lingkar Kepala | Berbasis deteksi kontur                      | Tidak tersedia (perangkat khusus)       |
| Kenyamanan Balita      | Tidak memerlukan kontak fisik                | Diperlukan kontak fisik                 |
| Biaya                  | Lebih rendah (kamera standar)                | Lebih tinggi (sensor fisik)             |
| Fleksibilitas          | Fleksibel (bisa diintegrasikan di mana saja) | Terbatas pada alat khusus               |
| Sinkronisasi Data      | Real-time melalui aplikasi                   | Real-time ke cloud melalui protokol IoT |

## 📈 Manfaat Bisnis dan Pengguna

##### 1. Efisiensi Biaya dan Model Berlangganan

Jalur _Computer Vision_ menawarkan solusi yang lebih hemat biaya, cocok untuk pasar kesehatan individu atau klinik kecil. Perusahaan kesehatan dapat menawarkan layanan ini dalam bentuk langganan aplikasi yang memungkinkan akses data dan riwayat kesehatan balita.

##### 2. Peningkatan Aksesibilitas Kesehatan

Dengan ketersediaan teknologi _Computer Vision_, keluarga dapat memantau kesehatan anak secara mandiri dari rumah tanpa perlu ke klinik. Ini membantu akses kesehatan yang lebih merata, terutama di daerah terpencil atau yang sulit dijangkau.

##### 3. Kemudahan untuk Tenaga Kesehatan

Sistem ini menyediakan data real-time untuk tenaga kesehatan, yang memungkinkan intervensi cepat jika terdeteksi indikasi masalah kesehatan. Sinkronisasi data secara langsung juga mempermudah pencatatan riwayat kesehatan untuk analisis jangka panjang.

## 📷 Gambar Pendukung dan Diagram

1. Diagram Proses Jalur Computer Vision untuk Pengukuran Tinggi dan Lingkar Kepala

   ![Diagram Jalur Computer Vision](../assets/pengukuran%20tinggi%20bayi%20-%20computer%20vision.webp)  
   _Ilustrasi tahapan penggunaan teknologi *Computer Vision* untuk pengukuran tinggi dan lingkar kepala._

2. Diagram Arsitektur IoT untuk Jalur Smart Scale

   ![Diagram IoT Smart Scale](../assets/pengukuran%20tinggi%20bayi%20-%20benam.webp)  
   _Gambaran arsitektur IoT pada Smart Scale untuk pengukuran parameter kesehatan balita._

## 🛠️ Langkah Implementasi di Lapangan

1. Kebutuhan Infrastruktur.

   - Jalur _Computer Vision_: Memerlukan kamera standar, aplikasi pemrosesan gambar, dan kalibrasi ruang.
   - Jalur _Smart Scale IoT_: Memerlukan perangkat IoT khusus (sensor fisik untuk berat, tinggi, suhu, dll.).

2. Kebutuhan Pengembangan Perangkat Lunak.
   - Aplikasi dengan _UI_ (User Interface) yang intuitif untuk pemantauan kesehatan dan integrasi dengan _cloud_.
   - Penggunaan algoritma pengolahan data secara otomatis untuk pemantauan risiko kesehatan balita.

## 🎯 Kesimpulan dan Rekomendasi

Kedua jalur ini menawarkan pendekatan yang berbeda dalam pengukuran dan pemantauan kesehatan balita. Jalur _Computer Vision_ cocok untuk aplikasi yang lebih fleksibel dan terjangkau, ideal bagi keluarga atau klinik kecil yang membutuhkan solusi tanpa kontak. Sementara itu, jalur _Smart Scale IoT_ memberikan akurasi tinggi yang sangat tepat untuk penggunaan klinis dengan kebutuhan data yang detail.

[**<<< Kembali**](../README.md)
