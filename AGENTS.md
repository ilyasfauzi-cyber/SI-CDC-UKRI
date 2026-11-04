# AGENTS.md
# AI Coding Agent Instructions — SI CDC UKRI

## 1. Project Identity

Project Name: Sistem Informasi Career Development Center (SI CDC) UKRI.

Institution: Universitas Kebangsaan Republik Indonesia.

Project Type: Web-Based Information System.

Project Purpose:
Mengembangkan sistem informasi Career Development Center untuk menghubungkan mahasiswa, alumni, universitas, dan Dunia Usaha Dunia Industri (DUDI) dalam layanan pengembangan karier, pengelolaan portofolio, lowongan pekerjaan, kemitraan industri, dan tracer study.

Seluruh pengembangan harus mengacu pada dokumen KAK, Project Plan, dan SRS yang tersedia di direktori `docs/`.

## 2. Technology Stack

Gunakan teknologi berikut:

- Backend: Laravel (PHP).
- Frontend: Blade.
- CSS Framework: Tailwind CSS.
- Database: MySQL.
- Local Development Environment: Laragon.
- Version Control: Git.
- Repository Hosting: GitHub.

Jangan mengganti teknologi utama tanpa persetujuan pemilik proyek.

## 3. System Actors and Roles

Sistem memiliki lima aktor utama:

### Super Admin
- Mengelola akun administrator.
- Mengelola role dan hak akses.
- Mengelola konfigurasi sistem.
- Melihat log aktivitas.

### Admin CDC
- Mengelola data mahasiswa dan alumni.
- Mengelola data mitra DUDI.
- Memverifikasi akun mitra.
- Memverifikasi lowongan pekerjaan.
- Memverifikasi data portofolio.
- Mengelola promosi talenta.
- Mengakses laporan dan analitik.

### Perwakilan DUDI
- Melakukan registrasi mitra.
- Mengelola profil perusahaan.
- Mengelola lowongan pekerjaan dan magang.
- Melihat dan meninjau lamaran.

### Mahasiswa dan Alumni
- Login dan mengelola profil.
- Mengelola portofolio.
- Mengunggah sertifikat dan pengalaman.
- Membuat serta mengunduh CV digital.
- Mencari dan melamar pekerjaan.
- Melacak status lamaran.
- Mengelola persetujuan penggunaan data pribadi.
- Mengisi tracer study sesuai ketentuan sistem.

### Pimpinan Universitas
- Melihat dashboard analitik.
- Melihat laporan tracer study.
- Memiliki hak akses read-only.

## 4. Main System Modules

Pengembangan sistem dibagi menjadi tiga modul:

### Module A: Profil dan Portofolio Talenta
Mencakup pengelolaan profil, portofolio, sertifikat, pengalaman, verifikasi data, dan CV digital.

### Module B: Lowongan dan Kemitraan DUDI
Mencakup pengelolaan mitra, lowongan pekerjaan, lowongan magang, pencarian pekerjaan, lamaran, pelacakan lamaran, dan promosi talenta.

### Module C: Analitik dan Tracer Study
Mencakup pengumpulan data tracer study, pengolahan data alumni, dashboard, dan laporan keterserapan alumni.

## 5. Development Rules

AI coding agent wajib mengikuti aturan berikut:

1. Baca dokumentasi proyek sebelum mengerjakan fitur.
2. Jangan membuat fitur di luar ruang lingkup tanpa persetujuan.
3. Jangan mengubah kebutuhan sistem secara sepihak.
4. Kerjakan fitur secara bertahap.
5. Gunakan penamaan variabel, class, function, dan file yang konsisten.
6. Hindari kode duplikat.
7. Gunakan prinsip modular dan mudah dipelihara.
8. Jangan menghapus kode yang sudah berfungsi tanpa alasan jelas.
9. Jangan mengubah konfigurasi penting tanpa persetujuan.
10. Dokumentasikan perubahan yang signifikan.

## 6. Database Rules

- Gunakan MySQL.
- Gunakan Laravel Migration untuk mengelola struktur database.
- Gunakan Eloquent ORM untuk interaksi database.
- Terapkan foreign key dan relasi yang sesuai.
- Hindari penyimpanan data yang tidak diperlukan.
- Gunakan validasi pada setiap input.
- Jangan menyimpan password dalam bentuk teks biasa.
- Perhatikan integritas dan konsistensi data.

## 7. Security and Privacy

Keamanan merupakan bagian penting dari sistem.

Wajib memperhatikan:

- Role-Based Access Control (RBAC).
- Password hashing.
- Validasi dan sanitasi input.
- Proteksi terhadap SQL Injection.
- Proteksi terhadap Cross-Site Scripting (XSS).
- Proteksi terhadap Cross-Site Request Forgery (CSRF).
- Penggunaan HTTPS pada deployment.
- Log aktivitas dan audit.
- Persetujuan pengguna sebelum data pribadi dibagikan kepada mitra DUDI.
- Mekanisme penarikan persetujuan (revoke consent).

Jangan pernah memasukkan password, API key, token, atau informasi rahasia ke repository.

## 8. UI/UX Guidelines

- Gunakan desain profesional dan konsisten.
- Gunakan Tailwind CSS.
- Buat tampilan responsif untuk desktop dan mobile.
- Gunakan navigasi yang mudah dipahami.
- Sesuaikan dashboard berdasarkan role pengguna.
- Gunakan komponen antarmuka yang dapat digunakan kembali.
- Berikan feedback untuk aksi berhasil, gagal, dan proses loading.

## 9. Testing Rules

Setiap fitur yang dikembangkan harus diuji.

Pengujian meliputi:

- Validasi input.
- Pengujian autentikasi.
- Pengujian hak akses berdasarkan role.
- Pengujian proses utama setiap fitur.
- Pengujian integrasi database.
- Pengujian tampilan responsif.

Jangan menyatakan fitur selesai jika belum diuji.

## 10. GitHub Workflow

Setiap pekerjaan harus terhubung dengan GitHub Issues jika Issues sudah tersedia.

Aturan:

- Gunakan branch terpisah untuk pekerjaan yang cukup besar.
- Gunakan commit message yang jelas.
- Hindari commit file konfigurasi rahasia.
- Jangan langsung mengubah branch utama tanpa memperhatikan aturan kolaborasi tim.
- Perbarui dokumentasi jika terjadi perubahan sistem.

Contoh commit:

- `feat: add user authentication`
- `feat: add student profile management`
- `fix: correct application status validation`
- `docs: update system documentation`
- `test: add authentication tests`

## 11. AI Agent Working Procedure

Sebelum mengerjakan tugas:

1. Periksa dokumentasi terkait.
2. Periksa struktur repository.
3. Pahami kebutuhan fitur.
4. Identifikasi file yang perlu dibuat atau diubah.
5. Jelaskan rencana pengerjaan.
6. Implementasikan perubahan.
7. Jalankan pengujian yang relevan.
8. Laporkan hasil pekerjaan dan file yang berubah.

Jangan langsung mengerjakan perubahan besar tanpa menjelaskan rencananya.

## 12. Important Restrictions

- Jangan mengganti Laravel, Blade, Tailwind CSS, atau MySQL tanpa persetujuan.
- Jangan mengarang kebutuhan sistem yang tidak tercantum dalam dokumen.
- Jangan menghapus data atau tabel tanpa persetujuan.
- Jangan melakukan deployment tanpa persetujuan.
- Jangan mengklaim pengujian berhasil jika belum dijalankan.
- Jika terdapat konflik antar dokumen, laporkan konflik dan minta keputusan sebelum mengubah kebutuhan.

## 13. Documentation Priority

Gunakan sumber berikut sebagai acuan:

1. KAK SI CDC UKRI untuk ruang lingkup dan tujuan proyek.
2. SRS SI CDC UKRI untuk kebutuhan perangkat lunak.
3. Project Plan untuk tahapan dan pembagian pekerjaan.
4. Gantt Chart untuk jadwal pengerjaan.

Jika terdapat perbedaan informasi, jangan mengambil keputusan sendiri. Laporkan perbedaannya terlebih dahulu.

---

End of AGENTS.md
