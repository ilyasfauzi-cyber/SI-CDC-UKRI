SI CDC UKRI

Sistem Informasi Career Development Center Universitas Kebangsaan Republik Indonesia

1. Deskripsi Proyek

SI CDC UKRI merupakan sistem informasi berbasis web yang dikembangkan untuk mendukung layanan Career Development Center (CDC) Universitas Kebangsaan Republik Indonesia.

Sistem ini bertujuan menghubungkan mahasiswa, alumni, pihak universitas, dan Dunia Usaha Dunia Industri (DUDI) melalui layanan pengelolaan profil karier, portofolio, informasi lowongan kerja, kemitraan industri, lamaran pekerjaan, serta tracer study alumni.

2. Tujuan Pengembangan

* Mempermudah mahasiswa dan alumni dalam mengelola profil serta portofolio karier.
* Menyediakan informasi lowongan kerja dan magang.
* Memfasilitasi kerja sama antara universitas dengan mitra DUDI.
* Mempermudah proses verifikasi data dan lowongan.
* Menyediakan informasi penelusuran alumni melalui tracer study.
* Membantu pihak universitas dalam memantau perkembangan karier dan keterserapan alumni.

3. Aktor Sistem

Sistem memiliki lima aktor utama:

Aktor	Hak Akses dan Tanggung Jawab
Super Admin	Mengelola akun admin, role, konfigurasi sistem, dan log aktivitas.
Admin CDC	Mengelola data mitra, memverifikasi lowongan dan portofolio, serta mengakses laporan.
Perwakilan DUDI	Mengelola profil perusahaan, mempublikasikan lowongan, dan meninjau lamaran.
Mahasiswa/Alumni	Mengelola profil, portofolio, CV, melamar pekerjaan, dan mengisi tracer study.
Pimpinan Universitas	Melihat dashboard analitik dan laporan tracer study.

4. Modul dan Fitur Utama

Pengembangan sistem dibagi menjadi tiga modul utama:

A. Profil dan Portofolio Talenta

* Pengelolaan profil mahasiswa dan alumni.
* Pengelolaan sertifikat, pelatihan, seminar, organisasi, dan pengalaman kerja.
* Verifikasi data portofolio.
* Pembuatan dan pengunduhan CV digital.

B. Lowongan dan Kemitraan DUDI

* Pengelolaan data mitra industri.
* Registrasi dan verifikasi mitra DUDI.
* Publikasi dan verifikasi lowongan kerja atau magang.
* Pencarian dan pengajuan lamaran pekerjaan.
* Pelacakan status lamaran.
* Promosi talenta mahasiswa dan alumni.

C. Analitik dan Tracer Study

* Pengisian kuesioner tracer study alumni.
* Pengelolaan data hasil tracer study.
* Dashboard analitik keterserapan alumni.
* Laporan untuk Admin CDC dan pimpinan universitas.

5. Teknologi yang Digunakan

Komponen	Teknologi
Backend	Laravel (PHP)
Frontend	Blade
CSS Framework	Tailwind CSS
Database	MySQL
Local Development Server	Laragon
Version Control	Git
Repository	GitHub

6. Metodologi Pengembangan

Pengembangan proyek menggunakan pendekatan Waterfall sesuai Project Plan, dengan tahapan:

1. Inisiasi dan perencanaan proyek.
2. Analisis kebutuhan sistem.
3. Perancangan sistem.
4. Implementasi dan pengembangan.
5. Pengujian dan evaluasi.
6. Deployment dan penyelesaian proyek.

7. Struktur Repository

SI-CDC-UKRI/
├── README.md
├── AGENTS.md
├── CLAUDE.md
├── RULES.md
├── docs/
│   ├── KAK.docx
│   ├── PROJECT-PLAN.docx
│   ├── SRS.docx
│   ├── GANTT-CHART.xlsx
│   ├── analysis/
│   ├── design/
│   └── testing/
├── app/
├── database/
├── resources/
├── routes/
├── public/
├── tests/
└── progress/

Catatan: Struktur direktori aplikasi akan mengikuti struktur bawaan Laravel setelah proses instalasi.

8. Status Pengembangan

Proyek berada pada tahap persiapan repository dan pengembangan awal.

Tahapan	Status
Penyusunan KAK	Selesai
Project Charter dan Project Plan	Selesai
Penyusunan WBS	Selesai
Penyusunan SRS	Selesai
Gantt Chart	Selesai
Persiapan Repository GitHub	Dalam Proses
Analisis dan Desain Sistem	Belum Dimulai
Implementasi Sistem	Belum Dimulai
Pengujian Sistem	Belum Dimulai
Deployment	Belum Dimulai

Status akan diperbarui mengikuti perkembangan pengerjaan proyek.

9. Dokumentasi Proyek

Dokumen perencanaan dan pengembangan sistem disimpan di dalam direktori docs/, meliputi:

* Kerangka Acuan Kerja (KAK).
* Project Charter dan Project Plan.
* Work Breakdown Structure (WBS).
* Sprint Backlog.
* Gantt Chart.
* Software Requirements Specification (SRS).
* Dokumentasi desain dan pengujian sistem.

10. Tim Pengembang

Proyek ini dikembangkan sebagai bagian dari kegiatan akademik Universitas Kebangsaan Republik Indonesia.

⸻

SI CDC UKRI
Sistem Informasi Career Development Center
Universitas Kebangsaan Republik Indonesia
