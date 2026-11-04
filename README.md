# SI CDC UKRI
### Sistem Informasi Career Development Center Universitas Kebangsaan Republik Indonesia

## 1. Tentang Proyek

SI CDC UKRI merupakan sistem informasi Career Development Center yang dikembangkan untuk mendukung pengelolaan informasi karier, peluang kerja, kerja sama dengan dunia usaha dan dunia industri (DUDI), serta pelacakan alumni di lingkungan Universitas Kebangsaan Republik Indonesia.

Sistem ini bertujuan membantu mahasiswa dan alumni memperoleh informasi peluang karier, mempermudah perusahaan dalam menyampaikan lowongan pekerjaan, serta mendukung pengelolaan dan pemantauan data karier oleh pihak universitas.

Proyek ini dikembangkan sebagai bagian dari kegiatan pengembangan sistem informasi oleh tim SI CDC UKRI.

## 2. Tujuan Proyek

- Mempermudah mahasiswa dan alumni dalam memperoleh informasi lowongan pekerjaan.
- Menyediakan wadah pengelolaan profil dan portofolio mahasiswa serta alumni.
- Memfasilitasi kerja sama antara universitas dengan dunia usaha dan dunia industri.
- Membantu pengelolaan data tracer study alumni.
- Menyediakan informasi dan laporan terkait perkembangan karier alumni.

## 3. Modul Utama Sistem

### A. Talent Profile & Portfolio
Modul untuk mengelola profil, informasi pendidikan, keterampilan, pengalaman, dan portofolio mahasiswa maupun alumni.

### B. Job Vacancies & DUDI Partnerships
Modul untuk mengelola informasi lowongan pekerjaan dan hubungan kerja sama dengan perusahaan atau dunia usaha dan dunia industri.

### C. Analytics & Tracer Study
Modul untuk mengelola data tracer study serta menyajikan informasi dan analisis perkembangan karier alumni.

## 4. Pengguna Sistem

Sistem dirancang untuk mendukung lima jenis pengguna:

| Pengguna | Hak Akses Umum |
|---|---|
| Super Admin | Pengelolaan dan pengaturan keseluruhan sistem |
| Admin CDC | Pengelolaan layanan Career Development Center |
| DUDI Representative | Pengelolaan informasi perusahaan dan lowongan pekerjaan |
| Student / Alumni | Pengelolaan profil dan akses informasi karier |
| University Leadership | Melihat informasi, analisis, dan laporan |

Hak akses detail akan disesuaikan dengan kebutuhan sistem yang telah dianalisis.

## 5. Teknologi yang Digunakan

| Komponen | Teknologi |
|---|---|
| Backend | Laravel (PHP) |
| Frontend | Blade |
| CSS Framework | Tailwind CSS |
| Database | MySQL |
| Local Development | Laragon |
| Version Control | Git |
| Repository | GitHub |

## 6. Anggota Tim

| No. | Nama | Username GitHub | Peran |
|---|---|---|---|
| 1 | Muhammad Ilyas Fauzi | [ilyasfauzi-cyber](https://github.com/ilyasfauzi-cyber) | Project Leader / PM |
| 2 | Aldy Ramadani | [aldyrmdny-lab](https://github.com/aldyrmdny-lab) | System Analyst |
| 3 | Naufal Al Farros | [naufalalfarros](https://github.com/naufalalfarros) | Backend Developer |
| 4 | Muhammad Abdul Aziz | [mhmmdabdulazis05-tech](https://github.com/mhmmdabdulazis05-tech) | Backend Developer |
| 5 | Gilang Bungsu Putra Anugrah | [gilanganugrah08](https://github.com/gilanganugrah08) | Frontend Developer |
| 6 | Yunita Nur'aini | [yunita-nrn](https://github.com/yunita-nrn) | QA & Documentation |

## 7. Persyaratan Instalasi

Sebelum menjalankan proyek, pastikan perangkat telah memiliki:

- Laragon.
- PHP dengan versi yang sesuai dengan kebutuhan Laravel proyek.
- Composer.
- Node.js dan npm.
- MySQL.
- Git.
- Visual Studio Code atau editor kode lainnya.

## 8. Cara Instalasi dan Menjalankan Proyek

### A. Clone Repository

Buka terminal atau Git Bash, kemudian jalankan:

```bash
git clone https://github.com/ilyasfauzi-cyber/SI-CDC-UKRI.git
```

Masuk ke direktori proyek:

```bash
cd SI-CDC-UKRI
```

### B. Install Dependency

Install dependency PHP:

```bash
composer install
```

Install dependency frontend:

```bash
npm install
```

### C. Konfigurasi Environment

Salin file konfigurasi:

```bash
cp .env.example .env
```

Jika menggunakan Command Prompt Windows:

```cmd
copy .env.example .env
```

Buat application key:

```bash
php artisan key:generate
```

### D. Konfigurasi Database

1. Jalankan MySQL melalui Laragon.
2. Buka phpMyAdmin atau database manager.
3. Buat database dengan nama:

```text
si_cdc_ukri
```

4. Sesuaikan konfigurasi database di file `.env`:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=si_cdc_ukri
DB_USERNAME=root
DB_PASSWORD=
```

Sesuaikan username dan password dengan konfigurasi MySQL masing-masing.

### E. Jalankan Migration

Setelah database dikonfigurasi dan migration tersedia:

```bash
php artisan migrate
```

Jika proyek sudah memiliki seeder yang disiapkan untuk lingkungan pengembangan, jalankan:

```bash
php artisan db:seed
```

### F. Jalankan Aplikasi

Jalankan server Laravel:

```bash
php artisan serve
```

Jalankan Vite untuk pengembangan frontend:

```bash
npm run dev
```

Buka aplikasi melalui browser:

```text
http://127.0.0.1:8000
```

## 9. Alur Kolaborasi GitHub

Proyek menggunakan tiga jenis branch:

| Branch | Fungsi |
|---|---|
| `main` | Versi aplikasi yang stabil |
| `develop` | Integrasi pekerjaan seluruh anggota |
| `feature/*` | Pengembangan fitur tertentu |

Alur kerja:

1. Anggota mengambil tugas melalui GitHub Issues.
2. Membuat branch fitur dari `develop`.
3. Melakukan pengembangan sesuai tanggung jawab.
4. Melakukan commit dan push ke GitHub.
5. Mengajukan Pull Request ke `develop`.
6. Melakukan pemeriksaan dan pengujian.
7. PM mengatur integrasi dan rilis ke `main`.

Seluruh anggota wajib mengikuti ketentuan dalam file `RULES.md`.

## 10. Dokumentasi Proyek

Dokumentasi proyek mencakup:

- Kerangka Acuan Kerja (KAK).
- Project Plan.
- Software Requirements Specification (SRS).
- Work Breakdown Structure (WBS).
- Gantt Chart.
- Dokumentasi analisis dan desain sistem.
- Dokumentasi pengujian aplikasi.

Dokumentasi akan diperbarui mengikuti perkembangan proyek.

## 11. Status Pengembangan

<em>Project Status: In Development</em>

Proyek SI CDC UKRI masih dalam tahap pengembangan. Fitur dan dokumentasi akan diperbarui secara bertahap sesuai perencanaan dan hasil pekerjaan tim.

---

**SI CDC UKRI**  
Universitas Kebangsaan Republik Indonesia

Repository: https://github.com/ilyasfauzi-cyber/SI-CDC-UKRI.git
