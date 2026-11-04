# CLAUDE.md
# Claude Code Project Configuration — SI CDC UKRI

## 1. Project Overview

Project ini adalah Sistem Informasi Career Development Center (SI CDC) Universitas Kebangsaan Republik Indonesia.

Sistem dikembangkan untuk membantu mahasiswa, alumni, Admin CDC, mitra DUDI, dan pimpinan universitas dalam layanan pengembangan karier, pengelolaan portofolio, lowongan pekerjaan, lamaran, serta tracer study.

## 2. Mandatory Instructions

Sebelum melakukan pekerjaan apa pun, baca dan ikuti seluruh instruksi dalam:

`@AGENTS.md`

File tersebut merupakan pedoman utama pengembangan proyek.

Jika instruksi dalam file ini berbeda dengan AGENTS.md, ikuti AGENTS.md dan laporkan perbedaannya.

## 3. Technology Stack

Gunakan teknologi yang telah ditetapkan:

- Laravel (PHP) sebagai backend.
- Blade sebagai frontend templating.
- Tailwind CSS sebagai CSS framework.
- MySQL sebagai database.
- Laragon sebagai lingkungan pengembangan lokal.

Jangan mengganti teknologi tanpa persetujuan pemilik proyek.

## 4. Project Documentation

Sebelum mengimplementasikan fitur, periksa dokumentasi yang relevan di direktori `docs/`.

Dokumen utama:

- KAK: ruang lingkup dan tujuan sistem.
- SRS: kebutuhan fungsional dan nonfungsional.
- Project Plan: tahapan dan pembagian pekerjaan.
- Gantt Chart: jadwal proyek.

Jangan mengarang kebutuhan yang tidak tercantum dalam dokumentasi.

## 5. Coding Standards

- Gunakan struktur dan konvensi bawaan Laravel.
- Gunakan MVC dengan pemisahan tanggung jawab yang jelas.
- Gunakan Laravel Migration untuk perubahan database.
- Gunakan Eloquent ORM.
- Terapkan validasi pada input pengguna.
- Gunakan middleware untuk pembatasan hak akses.
- Buat kode modular dan mudah dipelihara.
- Hindari duplikasi kode.
- Gunakan Blade Components untuk elemen UI yang digunakan berulang.
- Gunakan Tailwind CSS secara konsisten.

## 6. Development Workflow

Untuk setiap pekerjaan:

1. Periksa kondisi repository terlebih dahulu.
2. Baca instruksi dan dokumentasi terkait.
3. Pahami kebutuhan pekerjaan.
4. Periksa GitHub Issue jika tersedia.
5. Jelaskan rencana implementasi.
6. Implementasikan kode sesuai ruang lingkup.
7. Jalankan pengujian yang relevan.
8. Periksa kembali perubahan.
9. Laporkan hasil pekerjaan.

Jangan mengubah banyak bagian sistem yang tidak berkaitan dengan pekerjaan.

## 7. Database and Security

- Gunakan MySQL.
- Pastikan relasi database konsisten.
- Jangan menyimpan password dalam bentuk teks biasa.
- Terapkan autentikasi dan RBAC.
- Lindungi data pribadi mahasiswa dan alumni.
- Terapkan mekanisme consent sebelum data dibagikan kepada mitra DUDI.
- Jangan menampilkan data yang tidak sesuai dengan hak akses pengguna.
- Jangan menyimpan credential atau secret di repository.

## 8. User Interface

Buat antarmuka yang:

- Profesional dan konsisten.
- Responsif untuk desktop dan mobile.
- Mudah digunakan oleh setiap aktor.
- Memiliki navigasi sesuai role.
- Memiliki notifikasi untuk proses berhasil maupun gagal.

## 9. Testing

Setiap fitur harus diuji sesuai kebutuhan.

Jangan menyatakan pekerjaan selesai jika pengujian belum dilakukan.

Jika pengujian gagal, jelaskan penyebab dan langkah perbaikannya.

## 10. Communication

Gunakan Bahasa Indonesia untuk penjelasan kepada pemilik proyek.

Ketika menyelesaikan pekerjaan, berikan laporan yang mencakup:

- Ringkasan pekerjaan.
- File yang dibuat atau diubah.
- Fitur yang berhasil diimplementasikan.
- Pengujian yang telah dilakukan.
- Hasil pengujian.
- Kendala atau pekerjaan yang belum selesai.

Jika ada informasi yang belum jelas, tanyakan terlebih dahulu daripada membuat asumsi sendiri.

---

End of CLAUDE.md
