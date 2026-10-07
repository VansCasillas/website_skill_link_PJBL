<p align="center">
  <h1 align="center">Project Skill Link</h1>
  <p align="center">
    <strong>Platform Kolaborasi Mahasiswa Berbasis Skill, Proyek, dan Portofolio Prestasi</strong>
  </p>
</p>

---

## 📌 Tentang Project Skill Link

**Project Skill Link** adalah platform digital yang dirancang untuk membantu mahasiswa menemukan dan terhubung dengan mahasiswa lain berdasarkan *skill*, minat, pengalaman, dan kebutuhan proyek.

Selain sebagai media pencarian tim kolaborasi, platform ini juga menyediakan informasi kompetisi serta fitur untuk menyimpan sertifikat dan pencapaian mahasiswa sebagai portofolio digital.

### ❓ Permasalahan
Mahasiswa sering mengalami kesulitan dalam:
- Mencari rekan tim yang memiliki *skill* spesifik.
- Membentuk tim untuk tugas, proyek, atau kompetisi.
- Menemukan mahasiswa dengan minat yang selaras.
- Memperoleh informasi kompetisi/lomba secara terpusat.
- Menyimpan dan menampilkan bukti prestasi/sertifikat secara terstruktur.

### 💡 Solusi
Project Skill Link menyediakan tiga pilar utama:
1. **Skill Matching**: Fitur pencarian dan pencocokan mahasiswa berdasarkan keahlian.
2. **Project & Competition**: Wadah publikasi kebutuhan proyek serta informasi kompetisi.
3. **Achievement Portfolio**: Media penyimpanan sertifikat dan rekaman portofolio prestasi.

---

## 🛠️ Metodologi Pengembangan

Proyek ini dikembangkan dengan menerapkan kombinasi **Project Based Learning (PjBL)**, **Agile**, dan **Scrum**:

### Langkah-langkah Instalasi

1.  **Clone Repository:**
    ```bash
    git clone [URL_REPOSITORY_ANDA]
    cd nama-folder-proyek
    ```

2.  **Install Dependencies:**
    Gunakan Composer untuk menginstal semua paket PHP yang dibutuhkan.
    ```bash
    composer install
    ```

3.  **Konfigurasi Environment:**
    * Buat file `.env` dari contoh yang ada:
        ```bash
        cp .env.example .env
        ```
    * Buka file `.env` dan atur konfigurasi database Anda:
        ```dotenv
        APP_NAME="Jurnal PKL Digital"
        APP_ENV=local
        APP_KEY= # Akan diisi pada langkah berikutnya

        DB_CONNECTION=mysql
        DB_HOST=127.0.0.1
        DB_PORT=3306
        DB_DATABASE=[NAMA_DB_ANDA]
        DB_USERNAME=[USER_DB_ANDA]
        DB_PASSWORD=[PASS_DB_ANDA]
        ```

4.  **Generate Application Key:**
    ```bash
    php artisan key:generate
    ```

5.  **Migrasi Database:**
    Jalankan migrasi untuk membuat semua tabel.
    ```bash
    php artisan migrate
    ```
    **(Opsional: Jika Anda memiliki Seeder untuk data awal seperti akun Admin, jalankan: `php artisan db:seed`)*

6.  **Jalankan Server Lokal:**
    ```bash
    php artisan serve
    ```
    Aplikasi sekarang dapat diakses di `http://127.0.0.1:8000`.

---