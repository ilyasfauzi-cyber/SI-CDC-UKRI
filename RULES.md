# RULES.md
# ATURAN KERJA TIM SI CDC UKRI

## 1. Informasi Proyek

**Nama Proyek:** Sistem Informasi Career Development Center (SI CDC UKRI)  
**Repository:** https://github.com/ilyasfauzi-cyber/SI-CDC-UKRI  
**Teknologi:** Laravel (PHP), Blade, Tailwind CSS, MySQL  
**Local Development:** Laragon  
**Version Control:** Git dan GitHub

Dokumen ini berisi aturan kerja yang wajib diikuti seluruh anggota tim selama pengembangan SI CDC UKRI.

## 2. Struktur Tim dan Tanggung Jawab

| Nama | Username GitHub | Peran |
|---|---|---|
| Muhammad Ilyas Fauzi | ilyasfauzi-cyber | Project Leader / PM |
| Aldy Ramadani | aldyrmdny-lab | System Analyst |
| Naufal Al Farros | naufalalfarros | Backend Developer |
| Muhammad Abdul Aziz | mhmmdabdulazis05-tech | Backend Developer |
| Gilang Bungsu Putra Anugrah | gilanganugrah08 | Frontend Developer |
| Yunita Nur'aini | yunita-nrn | QA & Documentation |

### Tanggung Jawab

**Project Leader / PM — Muhammad Ilyas Fauzi**
- Mengatur pembagian pekerjaan dan prioritas.
- Mengelola GitHub Issues dan Milestones.
- Memantau perkembangan proyek.
- Mengawasi integrasi pekerjaan tim.
- Menyetujui Pull Request menuju branch utama.

**System Analyst — Aldy Ramadani**
- Menganalisis kebutuhan sistem.
- Menyusun alur proses dan kebutuhan fungsional.
- Menyusun dokumentasi analisis sistem.
- Berkoordinasi dengan developer mengenai kebutuhan fitur.

**Backend Developer — Naufal Al Farros dan Muhammad Abdul Aziz**
- Mengembangkan backend menggunakan Laravel.
- Mengelola database MySQL dan migration.
- Mengembangkan autentikasi, validasi, dan logika bisnis.
- Mengintegrasikan backend dengan frontend.

**Frontend Developer — Gilang Bungsu Putra Anugrah**
- Mengembangkan antarmuka menggunakan Blade dan Tailwind CSS.
- Membuat halaman dan komponen antarmuka.
- Memastikan tampilan responsif.
- Mengintegrasikan tampilan dengan data dari backend.

**QA & Documentation — Yunita Nur'aini**
- Menyusun skenario dan test case.
- Melakukan pengujian fitur.
- Mencatat bug dan hasil pengujian.
- Memelihara dokumentasi proyek.
- Melaporkan hasil pengujian kepada PM dan developer.

## 3. Aturan Branch Git

Repository menggunakan tiga jenis branch utama:

| Branch | Fungsi |
|---|---|
| `main` | Versi aplikasi yang stabil |
| `develop` | Integrasi seluruh pekerjaan tim |
| `feature/*` | Pengembangan fitur tertentu |

### Ketentuan

1. Branch `main` tidak boleh digunakan untuk pekerjaan harian.
2. Seluruh branch fitur dibuat dari `develop`.
3. Setiap anggota mengerjakan tugas melalui branch masing-masing.
4. Setelah selesai, perubahan diajukan melalui Pull Request menuju `develop`.
5. Branch `main` hanya diperbarui setelah integrasi dan pengujian dinyatakan layak oleh PM.
6. Dilarang melakukan force push pada branch bersama.

### Contoh Nama Branch

- `feature/authentication`
- `feature/student-profile`
- `feature/job-vacancies`
- `feature/dudi-partnership`
- `feature/dashboard`
- `feature/tracer-study`
- `fix/login-validation`
- `docs/project-documentation`

## 4. Alur Kerja GitHub

Urutan kerja setiap anggota:

1. Ambil pekerjaan melalui GitHub Issues.
2. Pastikan tugas dan ruang lingkup pekerjaan dipahami.
3. Ambil perubahan terbaru dari `develop`.
4. Buat branch baru dari `develop`.
5. Kerjakan fitur sesuai tanggung jawab.
6. Lakukan pengujian sebelum melakukan push.
7. Commit dan push perubahan ke GitHub.
8. Buat Pull Request dari branch fitur menuju `develop`.
9. Cantumkan deskripsi pekerjaan dan hasil pengujian.
10. Tunggu pemeriksaan dan persetujuan sebelum perubahan digabungkan.

### Contoh Perintah Git

```bash
git checkout develop
git pull origin develop

git checkout -b feature/nama-fitur

# Kerjakan perubahan kode

git add .
git commit -m "feat(auth): add login validation"
git push -u origin feature/nama-fitur
```

Setelah itu, buat Pull Request melalui GitHub.

## 5. Aturan Commit

Tim menggunakan format Conventional Commits:

```text
type(scope): deskripsi perubahan
```

Jenis commit:

| Type | Penggunaan |
|---|---|
| `feat` | Menambahkan fitur baru |
| `fix` | Memperbaiki bug |
| `docs` | Mengubah dokumentasi |
| `style` | Perubahan format atau tampilan kode tanpa mengubah logika |
| `refactor` | Merapikan struktur kode |
| `test` | Menambahkan atau memperbaiki pengujian |
| `chore` | Pemeliharaan proyek dan konfigurasi |

Contoh:

```text
feat(auth): add login feature
feat(student): add student profile page
fix(auth): fix login validation
docs(readme): update installation guide
test(job): add job vacancy test
```

Gunakan pesan commit yang jelas dan sesuai perubahan sebenarnya.

## 6. Aturan Pull Request

Setiap Pull Request wajib mencantumkan:

- Judul perubahan yang jelas.
- Ringkasan pekerjaan.
- Nomor atau tautan GitHub Issue.
- Daftar file atau bagian yang diubah.
- Langkah pengujian.
- Hasil pengujian.
- Screenshot apabila perubahan berkaitan dengan antarmuka.

### Ketentuan Review

1. Pull Request menuju `develop` harus diperiksa sebelum di-merge.
2. Minimal satu anggota lain melakukan pemeriksaan.
3. PM bertanggung jawab memastikan integrasi pekerjaan.
4. Perbaiki konflik dan kesalahan sebelum merge.
5. Jangan menggabungkan kode yang belum diuji.
6. PM mengatur merge dari `develop` ke `main`.

## 7. Aturan Pengembangan Aplikasi

Seluruh anggota wajib mengikuti teknologi yang telah ditentukan:

- Backend: Laravel (PHP).
- Frontend: Blade dan Tailwind CSS.
- Database: MySQL.
- Local Development: Laragon.

Ketentuan pengembangan:

1. Gunakan struktur folder dan standar Laravel yang konsisten.
2. Gunakan migration untuk perubahan struktur database.
3. Gunakan seeder untuk data awal atau data pengujian.
4. Hindari menulis kode yang sama berulang kali jika dapat dibuat menjadi komponen atau fungsi yang dapat digunakan kembali.
5. Jangan mengubah fitur atau kebutuhan sistem tanpa koordinasi dengan PM dan System Analyst.
6. Pastikan perubahan tidak merusak fitur yang sudah berjalan.

## 8. Aturan Pengujian dan Dokumentasi

1. Setiap developer wajib menguji kode sebelum mengajukan Pull Request.
2. QA bertugas memeriksa fitur berdasarkan kebutuhan sistem.
3. Setiap bug harus dicatat dan dilaporkan melalui GitHub Issues.
4. Bug yang ditemukan harus memiliki deskripsi dan langkah reproduksi.
5. Dokumentasi harus diperbarui apabila terdapat perubahan fitur, konfigurasi, atau alur sistem.
6. Hasil pengujian harus dapat dipahami dan diperiksa anggota lain.

## 9. Aturan Penggunaan AI

AI dapat digunakan untuk membantu proses pengembangan, seperti:

- Membantu menulis dan memahami kode.
- Membantu mencari penyebab error.
- Membantu menyusun dokumentasi.
- Membantu membuat test case.
- Membantu memberikan saran perbaikan kode.

Namun, setiap anggota wajib:

1. Memahami kode yang dihasilkan AI sebelum menggunakannya.
2. Memeriksa kesesuaian kode dengan kebutuhan proyek.
3. Menguji kode sebelum melakukan commit.
4. Tidak menyerahkan hasil AI tanpa pemeriksaan.
5. Tidak memasukkan informasi rahasia proyek ke layanan AI yang tidak diizinkan.

## 10. Keamanan Repository

Dilarang mengunggah:

- File `.env`.
- Password dan kredensial database.
- API key dan token autentikasi.
- Private key atau sertifikat rahasia.
- Informasi pribadi pengguna yang bersifat sensitif.

Gunakan `.env.example` untuk memberikan contoh konfigurasi tanpa menyertakan kredensial asli.

Pastikan file rahasia sudah tercantum dalam `.gitignore`.

## 11. Pelaporan Progres

Setiap anggota wajib memperbarui progres pekerjaan melalui GitHub Issues atau dokumentasi progres yang disepakati tim.

Informasi progres minimal:

- Nama anggota.
- Tugas atau Issue yang dikerjakan.
- Branch yang digunakan.
- Pekerjaan yang telah diselesaikan.
- Status pekerjaan.
- Kendala yang ditemukan.

Status pekerjaan:

- `To Do`
- `In Progress`
- `Review`
- `Done`
- `Blocked`

Jika mengalami kendala, segera komunikasikan kepada PM agar tidak menghambat pekerjaan anggota lain.

## 12. Prinsip Kerja Tim

1. Komunikasikan perubahan sebelum mengubah bagian pekerjaan anggota lain.
2. Jangan menghapus atau menimpa pekerjaan anggota lain tanpa persetujuan.
3. Patuhi pembagian tanggung jawab.
4. Saling melakukan pemeriksaan kode dan pengujian.
5. Utamakan kestabilan aplikasi daripada kecepatan menyelesaikan fitur.
6. Semua anggota bertanggung jawab terhadap kualitas hasil akhir SI CDC UKRI.

---

**Dokumen ini menjadi pedoman kerja seluruh anggota tim SI CDC UKRI selama proses pengembangan proyek.**
