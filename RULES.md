# RULES.md
# PROJECT DEVELOPMENT RULES — SI CDC UKRI

## 1. General Rules

1. Seluruh anggota tim wajib memahami tujuan dan ruang lingkup proyek SI CDC UKRI.
2. Setiap pekerjaan harus mengacu pada dokumen KAK, SRS, Project Plan, dan Gantt Chart.
3. Setiap perubahan kebutuhan sistem harus didiskusikan dan disetujui oleh tim.
4. Setiap anggota bertanggung jawab terhadap tugas yang diberikan.
5. Dilarang menghapus atau mengubah pekerjaan anggota lain tanpa koordinasi.
6. Komunikasi dan perkembangan pekerjaan harus dicatat dengan jelas.

## 2. Technology Rules

Teknologi yang digunakan dalam proyek:

- Backend: Laravel (PHP).
- Frontend: Blade.
- CSS Framework: Tailwind CSS.
- Database: MySQL.
- Local Development: Laragon.
- Version Control: Git.
- Repository: GitHub.

Pergantian teknologi harus mendapatkan persetujuan tim dan disesuaikan dengan dokumentasi proyek.

## 3. GitHub Repository Rules

1. Branch utama menggunakan nama `main`.
2. Jangan mengerjakan fitur langsung pada branch `main` jika pekerjaan dilakukan melalui branch fitur.
3. Setiap fitur atau perbaikan besar sebaiknya menggunakan branch tersendiri.
4. Setiap perubahan harus memiliki commit message yang jelas.
5. Gunakan GitHub Issues untuk mencatat dan melacak pekerjaan.
6. Hubungkan Pull Request dengan Issue terkait.
7. Perubahan penting harus diperiksa sebelum digabungkan ke branch utama.

### Branch Naming Convention

Gunakan format:

- `feature/nama-fitur`
- `fix/nama-perbaikan`
- `docs/nama-dokumentasi`
- `test/nama-pengujian`

Contoh:

- `feature/user-authentication`
- `feature/student-profile`
- `fix/application-validation`
- `docs/project-documentation`

## 4. Commit Message Rules

Gunakan format:

`type: description`

Jenis commit:

| Type | Penggunaan |
|---|---|
| feat | Menambahkan fitur |
| fix | Memperbaiki bug |
| docs | Mengubah dokumentasi |
| style | Mengubah tampilan atau format kode tanpa mengubah logika |
| refactor | Merapikan kode |
| test | Menambahkan atau memperbaiki pengujian |
| chore | Konfigurasi dan pemeliharaan proyek |

Contoh:

- `feat: add authentication system`
- `feat: add student profile management`
- `fix: correct job application status`
- `docs: update project documentation`
- `test: add user authentication tests`

## 5. Coding Standards

1. Gunakan struktur kode Laravel yang konsisten.
2. Pisahkan tanggung jawab Controller, Model, View, dan Service jika diperlukan.
3. Gunakan penamaan class dan method yang mudah dipahami.
4. Hindari kode duplikat.
5. Gunakan Laravel Migration untuk perubahan struktur database.
6. Gunakan validasi Laravel untuk setiap input.
7. Gunakan Eloquent ORM untuk interaksi database.
8. Jangan menuliskan query atau logika bisnis secara sembarangan di Blade.
9. Gunakan komponen Blade yang dapat digunakan kembali jika sesuai.
10. Pastikan kode mudah dibaca dan dipelihara.

## 6. Database Rules

1. Database utama menggunakan MySQL.
2. Setiap perubahan struktur tabel harus menggunakan Migration.
3. Gunakan relasi dan foreign key sesuai kebutuhan.
4. Gunakan Seeder untuk data awal atau data pengujian.
5. Jangan menghapus data penting tanpa persetujuan.
6. Gunakan nama tabel dan kolom secara konsisten.
7. Pastikan integritas data tetap terjaga.
8. Jangan menyimpan password dalam bentuk teks biasa.

## 7. Security Rules

1. Setiap halaman harus memeriksa autentikasi dan hak akses.
2. Terapkan Role-Based Access Control (RBAC).
3. Jangan memberikan akses melebihi kewenangan role pengguna.
4. Validasi seluruh input dari pengguna.
5. Jangan menampilkan informasi sensitif kepada pihak yang tidak berwenang.
6. Jangan menyimpan password, API key, token, atau credential di repository.
7. Gunakan file `.env` untuk konfigurasi rahasia.
8. Jangan mengunggah file `.env` ke GitHub.
9. Terapkan perlindungan CSRF, XSS, dan SQL Injection.
10. Data pribadi mahasiswa dan alumni hanya boleh dibagikan sesuai persetujuan dan kewenangan yang berlaku.

## 8. UI/UX Rules

1. Gunakan Tailwind CSS sebagai framework styling.
2. Tampilan harus responsif untuk desktop dan mobile.
3. Gunakan desain yang konsisten di seluruh halaman.
4. Navigasi harus mudah dipahami.
5. Dashboard harus menyesuaikan role pengguna.
6. Gunakan notifikasi untuk memberikan informasi keberhasilan atau kegagalan proses.
7. Form harus memiliki validasi dan pesan kesalahan yang jelas.

## 9. Testing Rules

Setiap fitur wajib diuji sebelum dinyatakan selesai.

Pengujian minimal meliputi:

- Pengujian autentikasi.
- Pengujian hak akses pengguna.
- Pengujian validasi form.
- Pengujian proses utama fitur.
- Pengujian penyimpanan dan pengambilan data.
- Pengujian integrasi antarfitur jika diperlukan.

Bug yang ditemukan harus dicatat melalui GitHub Issues.

Jangan menyatakan pengujian berhasil jika belum benar-benar dijalankan.

## 10. GitHub Issues and Pull Request Rules

1. Setiap pekerjaan harus memiliki Issue jika sistem pelacakan pekerjaan sudah digunakan.
2. Issue harus memiliki judul dan deskripsi yang jelas.
3. Setiap Issue harus memiliki kategori atau label yang sesuai.
4. Issue yang selesai harus diperbarui statusnya.
5. Pull Request harus menjelaskan perubahan yang dilakukan.
6. Pull Request harus menyertakan referensi Issue terkait.
7. Periksa konflik sebelum melakukan merge.
8. Jangan melakukan merge perubahan yang belum diperiksa.

## 11. Team Collaboration Rules

1. Setiap anggota wajib memperbarui progres pekerjaan.
2. Jika mengalami kendala, segera komunikasikan kepada tim.
3. Hindari mengerjakan file yang sama secara bersamaan tanpa koordinasi.
4. Lakukan sinkronisasi perubahan sebelum memulai pekerjaan.
5. Berikan informasi yang jelas ketika menyerahkan pekerjaan kepada anggota lain.
6. Setiap keputusan penting harus didokumentasikan.

## 12. AI Assistant Rules

Claude Code dan AI coding assistant lainnya harus:

1. Membaca `AGENTS.md` dan dokumentasi proyek sebelum mengerjakan tugas.
2. Mengikuti teknologi yang telah ditentukan.
3. Tidak membuat fitur di luar ruang lingkup tanpa persetujuan.
4. Tidak mengubah struktur database secara sembarangan.
5. Tidak menghapus kode atau file penting tanpa persetujuan.
6. Menjelaskan rencana sebelum perubahan besar.
7. Menjalankan pengujian yang relevan setelah implementasi.
8. Melaporkan file yang dibuat atau diubah.
9. Melaporkan kendala dan bug yang ditemukan.
10. Tidak mengklaim pekerjaan selesai jika belum diverifikasi.

## 13. Definition of Done

Pekerjaan dapat dinyatakan selesai apabila:

- Kebutuhan pada Issue telah dipenuhi.
- Implementasi sesuai dokumentasi proyek.
- Tidak ada error yang diketahui dan belum ditangani.
- Pengujian yang relevan telah dijalankan.
- Perubahan telah disimpan ke Git.
- Dokumentasi diperbarui jika diperlukan.
- Status Issue telah diperbarui.

---

**Project:** SI CDC UKRI  
**Institution:** Universitas Kebangsaan Republik Indonesia  
**Document:** Project Development Rules
