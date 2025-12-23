# 🌾 SiKepang - Sistem Informasi Ketahanan Pangan Kota Ternate

![SiKepang Banner](path/to/your/screenshot.png) **SiKepang** adalah platform digital yang dirancang untuk membantu Dinas Ketahanan Pangan dan masyarakat Kota Ternate dalam memantau ketersediaan (stok), stabilitas harga, dan distribusi bahan pokok. Aplikasi ini menyajikan data secara transparan, *real-time*, dan berbasis lokasi (GIS).

## 🚀 Fitur Utama

### 1. 📊 Dashboard Monitoring Eksekutif
- Visualisasi tren ketersediaan stok pangan selama satu tahun (Januari - Desember) menggunakan **Chart.js**.
- Indikator visual untuk stok melimpah atau menipis.
- Ringkasan data komoditas utama (Beras, Cabai, Daging, dll).

### 2. 🗺️ Peta Sebaran Mitra (GIS)
- Integrasi **Mapbox GL JS** untuk memetakan lokasi pasar, distributor, dan mitra pangan.
- **Interactive Popup:** Menampilkan detail toko, alamat, kontak WhatsApp, dan kategori usaha.
- **Direct Routing:** Fitur navigasi langsung ke lokasi mitra via Google Maps.

### 3. 📝 Manajemen Data Pangan
- Pencatatan data stok masuk dan keluar per komoditas.
- Filter data berdasarkan kategori dinas dan waktu.
- Dukungan data presisi tinggi (Tonase dengan desimal).

### 4. 📄 Laporan & Ekspor
- Cetak laporan ketersediaan pangan otomatis ke format **PDF**.
- Laporan siap cetak untuk kebutuhan administrasi dinas.

---

## 🛠️ Teknologi yang Digunakan

Project ini dibangun dengan *Tech Stack* modern dan efisien:

* **Backend Framework:** [CodeIgniter 4](https://codeigniter.com/) (PHP)
* **Database:** MySQL / MariaDB
* **Frontend:** HTML5, CSS3, [Bootstrap 5](https://getbootstrap.com/)
* **Visualization:** [Chart.js](https://www.chartjs.org/) (Grafik Statistik)
* **Mapping API:** [Mapbox GL JS](https://www.mapbox.com/)
* **PDF Generator:** DomPDF

---

## 💻 Instalasi & Menjalankan Project

Ikuti langkah-langkah berikut untuk menjalankan project di komputer lokal (Localhost):

### Prasyarat
- PHP >= 7.4 (Disarankan PHP 8.1+)
- Composer
- Web Server (XAMPP/Laragon) atau built-in spark

### Langkah Instalasi

1.  **Clone Repositori**
    ```bash
    git clone [https://github.com/username-anda/sikepang.git](https://github.com/username-anda/sikepang.git)
    cd sikepang
    ```

2.  **Install Dependencies**
    ```bash
    composer install
    ```

3.  **Konfigurasi Database**
    - Buat database baru di phpMyAdmin bernama `sikepang_db`.
    - Ubah file `env` menjadi `.env`, lalu atur konfigurasi database:
      ```ini
      database.default.hostname = localhost
      database.default.database = sikepang_db
      database.default.username = root
      database.default.password =
      database.default.DBDriver = MySQLi
      ```

4.  **Migrasi & Seeding Data**
    Jalankan perintah berikut untuk membuat tabel dan mengisi data dummy/awal (termasuk data stok 2025):
    ```bash
    php spark migrate
    php spark db:seed DataStok2025
    ```

5.  **Jalankan Server**
    ```bash
    php spark serve
    ```

6.  **Akses Aplikasi**
    Buka browser dan kunjungi: `http://localhost:8080`

---

## 📸 Screenshots

| Dashboard Monitoring | Peta Sebaran |
| :---: | :---: |
| ![Dashboard](link_gambar_dashboard) | ![Peta](link_gambar_peta) |

*(Ganti teks ini dengan screenshot aplikasi Anda agar lebih menarik)*

---

## 🤝 Kontribusi & Kredit

Dikembangkan oleh **[Nama Anda]** sebagai bagian dari [Tugas Akhir/Project Kuliah/Portofolio].
Data bersumber dari **Dinas Ketahanan Pangan Kota Ternate** (Simulasi/Data Real).

---

Please ⭐ this repository if you find it useful!
