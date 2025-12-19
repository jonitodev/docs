# DOKUMENTASI PROYEK
# WEBSITE NCS LABORATORY
## Network & Cyber Security Laboratory
### Politeknik Negeri Malang

---

**Versi Dokumen:** 1.0  
**Tanggal:** Desember 2025  
**Status:** Final Release

---

# LEMBAR PENGESAHAN

| **Jabatan** | **Nama** | **Tanda Tangan** | **Tanggal** |
|-------------|----------|------------------|-------------|
| Pembimbing 1 | ........................ | ........................ | ........................ |
| Pembimbing 2 | ........................ | ........................ | ........................ |
| Penguji 1 | ........................ | ........................ | ........................ |
| Penguji 2 | ........................ | ........................ | ........................ |
| Ketua Program Studi | ........................ | ........................ | ........................ |

**Tim Pengembang (Total 5 Orang):**

| **No** | **Nama** | **NIM** | **Peran** |
|--------|----------|---------|-----------|
| 1 | ........................ | ........................ | Project Manager (PM) |
| 2 | ........................ | ........................ | Backend Developer |
| 3 | ........................ | ........................ | Frontend Developer |
| 4 | ........................ | ........................ | UI/UX Designer |
| 5 | ........................ | ........................ | UI/UX Designer |

---

# DAFTAR ISI

1. [Ringkasan Eksekutif](#ringkasan-eksekutif)  
2. [Pendahuluan](#pendahuluan)  
   - 2.1 [Latar Belakang](#21-latar-belakang)  
   - 2.2 [Rumusan Masalah](#22-rumusan-masalah)  
   - 2.3 [Tujuan Proyek](#23-tujuan-proyek)  
   - 2.4 [Ruang Lingkup Proyek](#24-ruang-lingkup-proyek)  
3. [Project Charter](#project-charter)  
   - 3.1 [Deskripsi Proyek](#31-deskripsi-proyek)  
   - 3.2 [Tujuan dan Sasaran](#32-tujuan-dan-sasaran)  
   - 3.3 [Ruang Lingkup](#33-ruang-lingkup)  
   - 3.4 [Pemangku Kepentingan](#34-pemangku-kepentingan)  
   - 3.5 [Success Criteria](#35-success-criteria)  
4. [Spesifikasi Kebutuhan Perangkat Lunak (SKPL)](#spesifikasi-kebutuhan-perangkat-lunak-skpl)  
   - 4.1 [Kebutuhan Fungsional](#41-kebutuhan-fungsional)  
   - 4.2 [Kebutuhan Non-Fungsional](#42-kebutuhan-non-fungsional)  
   - 4.3 [Diagram Pendukung](#43-diagram-pendukung)  
5. [Perencanaan Proyek](#perencanaan-proyek)  
   - 5.1 [Jadwal Proyek](#51-jadwal-proyek)  
   - 5.2 [Pembagian Tugas](#52-pembagian-tugas)  
   - 5.3 [Sumber Daya dan Anggaran](#53-sumber-daya-dan-anggaran)  
6. [Implementasi Proyek](#implementasi-proyek)  
   - 6.1 [Langkah-langkah Pelaksanaan](#61-langkah-langkah-pelaksanaan)  
   - 6.2 [Teknologi yang Digunakan](#62-teknologi-yang-digunakan)  
   - 6.3 [Tantangan dan Solusi](#63-tantangan-dan-solusi)  
7. [Dokumen Hasil Pengujian](#dokumen-hasil-pengujian)  
   - 7.1 [Metode Pengujian](#71-metode-pengujian)  
   - 7.2 [Hasil Pengujian](#72-hasil-pengujian)  
   - 7.3 [Evaluasi Terhadap Spesifikasi](#73-evaluasi-terhadap-spesifikasi)  
8. [Panduan Pengguna](#panduan-pengguna)  
   - 8.1 [Petunjuk Instalasi](#81-petunjuk-instalasi)  
   - 8.2 [Cara Penggunaan](#82-cara-penggunaan)  
   - 8.3 [Pemecahan Masalah](#83-pemecahan-masalah)  
9. [Kesimpulan dan Rekomendasi](#kesimpulan-dan-rekomendasi)  
10. [Referensi](#referensi)  
11. [Lampiran](#lampiran)  

---

# DAFTAR GAMBAR

| **No** | **Judul Gambar** | **Halaman** |
|--------|------------------|-------------|
| Gambar 2.1 | Logo NCS Laboratory | - |
| Gambar 4.1 | Use Case Diagram | - |
| Gambar 4.2 | Entity Relationship Diagram (ERD) | - |
| Gambar 4.3 | Data Flow Diagram Level 0 | - |
| Gambar 4.4 | Data Flow Diagram Level 1 | - |
| Gambar 4.5 | Arsitektur Sistem | - |
| Gambar 5.1 | Diagram Gantt | - |
| Gambar 6.1 | Struktur Folder Proyek | - |
| Gambar 6.2 | Tampilan Halaman Beranda | - |
| Gambar 6.3 | Tampilan Panel Admin Dashboard | - |
| Gambar 8.1 | Alur Instalasi Sistem | - |
| Gambar 8.2 | Tampilan Login Admin | - |

---

# DAFTAR TABEL

| **No** | **Judul Tabel** | **Halaman** |
|--------|-----------------|-------------|
| Tabel 3.1 | Pemangku Kepentingan | - |
| Tabel 4.1 | Kebutuhan Fungsional | - |
| Tabel 4.2 | Kebutuhan Non-Fungsional | - |
| Tabel 4.3 | Struktur Tabel Database | - |
| Tabel 5.1 | Jadwal Proyek | - |
| Tabel 5.2 | Pembagian Tugas Tim | - |
| Tabel 5.3 | Estimasi Anggaran | - |
| Tabel 6.1 | Stack Teknologi | - |
| Tabel 7.1 | Hasil Pengujian Fungsional | - |
| Tabel 7.2 | Hasil Pengujian Performa | - |

---

# RINGKASAN EKSEKUTIF

## Latar Belakang
Laboratorium Network & Cyber Security (NCS) Politeknik Negeri Malang memerlukan platform digital untuk mempublikasikan informasi, kegiatan, penelitian, dan layanan laboratorium kepada publik secara efektif dan profesional.

## Tujuan
Mengembangkan website profil laboratorium yang modern, responsif, dan mudah dikelola dengan fitur Content Management System (CMS) untuk administrator.

## Solusi
Website NCS Laboratory dibangun menggunakan arsitektur PHP Native dengan database PostgreSQL, framework CSS TailwindCSS, dan tema "Pastel Cyber" yang modern dengan efek visual Matrix Rain. Sistem dilengkapi panel administrasi lengkap untuk mengelola seluruh konten website.

## Hasil
- Website publik dengan 12+ halaman informatif
- Panel administrasi dengan 14+ modul CRUD
- Database dengan **14 tabel relasional**
- Tema responsif untuk semua perangkat
- Sistem keamanan dengan CSRF protection dan password hashing

## Dampak
- Meningkatkan visibilitas dan profesionalisme laboratorium
- Mempermudah akses informasi bagi mahasiswa dan publik
- Menyediakan arsip digital untuk penelitian dan pengabdian
- Memfasilitasi komunikasi melalui form kontak terintegrasi

---

# PENDAHULUAN

## 2.1 Latar Belakang

Laboratorium Network & Cyber Security (NCS) merupakan salah satu laboratorium unggulan di Jurusan Teknologi Informasi Politeknik Negeri Malang yang berfokus pada riset dan pengembangan di bidang keamanan jaringan dan siber. Laboratorium ini memiliki peran penting dalam:

1. **Penelitian:** Menghasilkan publikasi ilmiah di bidang cyber security  
2. **Pengabdian Masyarakat:** Memberikan pelatihan dan konsultasi keamanan siber  
3. **Pendidikan:** Menyediakan fasilitas praktikum untuk mahasiswa  
4. **Kolaborasi:** Menjalin kerjasama dengan industri dan institusi lain  

Seiring perkembangan teknologi informasi, kebutuhan akan platform digital untuk mempromosikan dan menginformasikan kegiatan laboratorium menjadi sangat penting. Website profil laboratorium diperlukan untuk:

- Mempublikasikan informasi profil, visi, misi, dan struktur organisasi  
- Menampilkan agenda kegiatan dan dokumentasi  
- Menyediakan arsip penelitian dan pengabdian masyarakat  
- Memfasilitasi layanan konsultasi dan sarana prasarana  
- Meningkatkan branding dan profesionalisme laboratorium  

## 2.2 Rumusan Masalah

1. Bagaimana merancang dan membangun website profil laboratorium yang informatif dan menarik?  
2. Bagaimana mengimplementasikan sistem manajemen konten yang mudah digunakan oleh administrator?  
3. Bagaimana memastikan website responsif dan dapat diakses dari berbagai perangkat?  
4. Bagaimana mengintegrasikan arsip penelitian dan pengabdian dengan fitur download?  
5. Bagaimana menerapkan standar keamanan web yang baik?  

## 2.3 Tujuan Proyek

### Tujuan Umum
Mengembangkan website profil NCS Laboratory yang profesional, modern, dan mudah dikelola.

### Tujuan Khusus
1. Membangun website frontend dengan desain responsif dan tema cyber security  
2. Mengembangkan panel administrasi dengan fitur CRUD lengkap  
3. Mengimplementasikan database relasional untuk penyimpanan data  
4. Menyediakan fitur upload dan download dokumen (PDF)  
5. Mengintegrasikan galeri multimedia (foto dan video)  
6. Menerapkan sistem autentikasi dan otorisasi pengguna  
7. Memastikan keamanan website dengan CSRF protection  

## 2.4 Ruang Lingkup Proyek

### Dalam Ruang Lingkup (In Scope)
- Website publik dengan halaman informatif  
- Panel administrasi dengan autentikasi  
- Manajemen konten (CRUD) untuk semua entitas  
- Upload dan download dokumen PDF  
- Galeri foto dan video  
- Form kontak pengunjung  
- Responsif untuk desktop, tablet, dan mobile  

### Di Luar Ruang Lingkup (Out of Scope)
- Integrasi payment gateway  
- Sistem e-learning  
- Forum diskusi online  
- Mobile application (native)  
- Multi-bahasa (i18n)  

---

# PROJECT CHARTER

## 3.1 Deskripsi Proyek

**Nama Proyek:** Website NCS Laboratory  
**Jenis Proyek:** Pengembangan Website Profil Institusi  
**Durasi:** 3 Bulan  
**Metodologi:** Waterfall dengan iterasi

Website NCS Laboratory adalah platform digital berbasis web yang berfungsi sebagai:
- **Company Profile:** Menampilkan informasi lengkap tentang laboratorium  
- **Content Management System:** Memungkinkan admin mengelola konten secara dinamis  
- **Digital Archive:** Menyimpan dan mendistribusikan dokumen penelitian/pengabdian  
- **Communication Hub:** Menyediakan saluran komunikasi dengan pengunjung  

## 3.2 Tujuan dan Sasaran

### Tujuan Bisnis
| **ID** | **Tujuan** | **Metrik Keberhasilan** |
|--------|------------|-------------------------|
| OBJ-01 | Meningkatkan visibilitas laboratorium | 1000+ pengunjung/bulan |
| OBJ-02 | Mempermudah akses informasi | 90% konten dapat diakses dalam 3 klik |
| OBJ-03 | Efisiensi pengelolaan konten | Admin dapat update konten dalam <5 menit |
| OBJ-04 | Arsip digital penelitian | 100% dokumen terdigitalisasi |

### Sasaran Teknis
| **ID** | **Sasaran** | **Target** |
|--------|-------------|------------|
| TECH-01 | Performa halaman | Load time <3 detik |
| TECH-02 | Responsivitas | Compatible dengan 95% browser modern |
| TECH-03 | Uptime | 99.5% availability |
| TECH-04 | Keamanan | 0 critical vulnerability |

## 3.3 Ruang Lingkup

### Deliverables
1. **Source Code:** Kode sumber lengkap dengan dokumentasi  
2. **Database Schema:** Struktur database PostgreSQL  
3. **User Manual:** Panduan penggunaan untuk admin  
4. **Technical Documentation:** Dokumentasi teknis sistem  
5. **Testing Report:** Laporan hasil pengujian  

### Fitur Utama

#### Frontend (Public)
| **Modul** | **Deskripsi** |
|-----------|---------------|
| Beranda | Landing page dengan hero section dan Matrix Rain effect |
| Visi & Misi | Halaman profil visi, misi, dan tujuan laboratorium |
| Struktur Organisasi | Struktur dan tim laboratorium |
| Bidang Fokus | Area fokus penelitian laboratorium |
| Roadmap | Timeline perkembangan laboratorium |
| Agenda | Kegiatan dan event mendatang |
| Galeri | Dokumentasi foto dan video |
| Penelitian | Arsip dokumen penelitian (PDF) |
| Pengabdian | Arsip dokumen pengabdian masyarakat (PDF) |
| Sarana | Informasi fasilitas dan prasarana |
| Konsultatif | Layanan konsultasi yang tersedia |
| Link Terkait | Link eksternal terkait |
| Kontak | Form kontak pengunjung |

#### Backend (Admin Panel)
| **Modul** | **Operasi CRUD** |
|-----------|------------------|
| Dashboard | Statistik dan overview |
| Settings | Konfigurasi website |
| Users | Manajemen pengguna admin |
| Organization | Struktur organisasi |
| Team | Tim pengembang |
| Agenda | Kegiatan dan event |
| Gallery | Foto dan video |
| Documents | Dokumen PDF (penelitian/pengabdian) |
| Publications | Publikasi penelitian SINTA |
| Services | Layanan (sarana/konsultatif) |
| Focus Areas | Bidang fokus |
| Roadmap | Timeline/roadmap |
| Links | Link eksternal |
| Comments | Pesan pengunjung |

## 3.4 Pemangku Kepentingan

**Tabel 3.1: Pemangku Kepentingan**

| **Stakeholder** | **Peran** | **Kepentingan** | **Pengaruh** |
|-----------------|-----------|-----------------|--------------|
| Kepala Lab NCS | Project Sponsor | Tinggi | Tinggi |
| Dosen Pembimbing | Advisor | Tinggi | Tinggi |
| Tim Pengembang | Developer | Tinggi | Tinggi |
| Admin Website | End User (Admin) | Tinggi | Sedang |
| Mahasiswa | End User (Public) | Sedang | Rendah |
| Pengunjung Umum | End User (Public) | Sedang | Rendah |
| JTI Polinema | Stakeholder Institusi | Sedang | Sedang |

## 3.5 Success Criteria

### Kriteria Penerimaan Proyek
1. ✅ Semua fitur dalam scope berhasil diimplementasikan  
2. ✅ Website dapat diakses secara online (melalui IP VPS)  
3. ✅ Panel admin berfungsi dengan baik  
4. ✅ Dokumentasi lengkap tersedia  
5. ✅ Tidak ada bug critical dan high  
6. ✅ Performance test memenuhi target  
7. ✅ Security test tidak menemukan vulnerability critical  

### Key Performance Indicators (KPI)
| **KPI** | **Target** | **Metode Pengukuran** |
|---------|------------|----------------------|
| Code Quality | Grade A/B | Code review & linting |
| Test Coverage | >80% | Unit & integration test |
| Bug Density | <5 bugs/KLOC | Bug tracking |
| Performance | PageSpeed >80 | Google PageSpeed Insights |
| Security | No critical issues | OWASP testing |

---

# SPESIFIKASI KEBUTUHAN PERANGKAT LUNAK (SKPL)

## 4.1 Kebutuhan Fungsional

**Tabel 4.1: Kebutuhan Fungsional**

### Modul Autentikasi (FR-AUTH)
| **ID** | **Kebutuhan** | **Prioritas** | **Status** |
|--------|---------------|---------------|------------|
| FR-AUTH-01 | Sistem menyediakan halaman login untuk admin | High | ✅ Implemented |
| FR-AUTH-02 | Sistem memvalidasi username dan password | High | ✅ Implemented |
| FR-AUTH-03 | Sistem menyediakan fitur logout | High | ✅ Implemented |
| FR-AUTH-04 | Sistem melindungi halaman admin dari akses unauthorized | High | ✅ Implemented |
| FR-AUTH-05 | Sistem mencatat waktu login terakhir pengguna | Medium | ✅ Implemented |

### Modul Dashboard (FR-DASH)
| **ID** | **Kebutuhan** | **Prioritas** | **Status** |
|--------|---------------|---------------|------------|
| FR-DASH-01 | Sistem menampilkan statistik jumlah dokumen | High | ✅ Implemented |
| FR-DASH-02 | Sistem menampilkan statistik jumlah galeri | High | ✅ Implemented |
| FR-DASH-03 | Sistem menampilkan statistik jumlah agenda | High | ✅ Implemented |
| FR-DASH-04 | Sistem menampilkan jumlah pesan belum dibaca | High | ✅ Implemented |
| FR-DASH-05 | Sistem menampilkan pesan terbaru | Medium | ✅ Implemented |
| FR-DASH-06 | Sistem menampilkan dokumen terbaru | Medium | ✅ Implemented |
| FR-DASH-07 | Sistem menyediakan quick action buttons | Low | ✅ Implemented |

### Modul Pengaturan (FR-SET)
| **ID** | **Kebutuhan** | **Prioritas** | **Status** |
|--------|---------------|---------------|------------|
| FR-SET-01 | Admin dapat mengubah nama dan tagline website | High | ✅ Implemented |
| FR-SET-02 | Admin dapat mengubah deskripsi website | High | ✅ Implemented |
| FR-SET-03 | Admin dapat mengubah informasi kontak | High | ✅ Implemented |
| FR-SET-04 | Admin dapat mengubah visi, misi, dan tujuan | High | ✅ Implemented |
| FR-SET-05 | Admin dapat mengubah link social media | Medium | ✅ Implemented |

### Modul Dokumen (FR-DOC)
| **ID** | **Kebutuhan** | **Prioritas** | **Status** |
|--------|---------------|---------------|------------|
| FR-DOC-01 | Admin dapat menambahkan dokumen PDF baru | High | ✅ Implemented |
| FR-DOC-02 | Admin dapat mengedit informasi dokumen | High | ✅ Implemented |
| FR-DOC-03 | Admin dapat menghapus dokumen | High | ✅ Implemented |
| FR-DOC-04 | Admin dapat mengkategorikan dokumen (penelitian/pengabdian) | High | ✅ Implemented |
| FR-DOC-05 | Sistem mencatat jumlah download dokumen | Medium | ✅ Implemented |
| FR-DOC-06 | Pengunjung dapat mengunduh dokumen PDF | High | ✅ Implemented |

### Modul Galeri (FR-GAL)
| **ID** | **Kebutuhan** | **Prioritas** | **Status** |
|--------|---------------|---------------|------------|
| FR-GAL-01 | Admin dapat mengunggah foto ke galeri | High | ✅ Implemented |
| FR-GAL-02 | Admin dapat mengunggah video ke galeri | High | ✅ Implemented |
| FR-GAL-03 | Admin dapat mengedit informasi galeri | High | ✅ Implemented |
| FR-GAL-04 | Admin dapat menghapus item galeri | High | ✅ Implemented |
| FR-GAL-05 | Pengunjung dapat melihat galeri foto dan video | High | ✅ Implemented |

### Modul Agenda (FR-AGD)
| **ID** | **Kebutuhan** | **Prioritas** | **Status** |
|--------|---------------|---------------|------------|
| FR-AGD-01 | Admin dapat menambahkan agenda baru | High | ✅ Implemented |
| FR-AGD-02 | Admin dapat mengedit agenda | High | ✅ Implemented |
| FR-AGD-03 | Admin dapat menghapus agenda | High | ✅ Implemented |
| FR-AGD-04 | Sistem menampilkan agenda mendatang di beranda | High | ✅ Implemented |
| FR-AGD-05 | Admin dapat menandai agenda sebagai featured | Medium | ✅ Implemented |

### Modul Pesan/Kontak (FR-MSG)
| **ID** | **Kebutuhan** | **Prioritas** | **Status** |
|--------|---------------|---------------|------------|
| FR-MSG-01 | Pengunjung dapat mengirim pesan melalui form kontak | High | ✅ Implemented |
| FR-MSG-02 | Sistem memvalidasi input form kontak | High | ✅ Implemented |
| FR-MSG-03 | Admin dapat melihat daftar pesan | High | ✅ Implemented |
| FR-MSG-04 | Admin dapat menandai pesan sebagai sudah dibaca | High | ✅ Implemented |
| FR-MSG-05 | Sistem mencatat IP address pengirim pesan | Medium | ✅ Implemented |

## 4.2 Kebutuhan Non-Fungsional

**Tabel 4.2: Kebutuhan Non-Fungsional**

### Performance (NFR-PERF)
| **ID** | **Kebutuhan** | **Target** | **Status** |
|--------|---------------|------------|------------|
| NFR-PERF-01 | Halaman harus dimuat dalam waktu <3 detik | 3 detik | ✅ Met |
| NFR-PERF-02 | Sistem dapat menangani 100 concurrent users | 100 users | ✅ Met |
| NFR-PERF-03 | Database query response <500ms | 500ms | ✅ Met |

### Security (NFR-SEC)
| **ID** | **Kebutuhan** | **Implementasi** | **Status** |
|--------|---------------|------------------|------------|
| NFR-SEC-01 | Proteksi CSRF untuk semua form | Token validation | ✅ Implemented |
| NFR-SEC-02 | Password hashing dengan bcrypt | PASSWORD_DEFAULT | ✅ Implemented |
| NFR-SEC-03 | Input sanitization untuk mencegah XSS | htmlspecialchars() | ✅ Implemented |
| NFR-SEC-04 | Prepared statements untuk mencegah SQL Injection | PDO prepared | ✅ Implemented |
| NFR-SEC-05 | Proteksi direktori sensitif | .htaccess rules | ✅ Implemented |
| NFR-SEC-06 | Environment variables untuk credentials | .env file | ✅ Implemented |

### Usability (NFR-USE)
| **ID** | **Kebutuhan** | **Target** | **Status** |
|--------|---------------|------------|------------|
| NFR-USE-01 | Responsif untuk semua ukuran layar | Mobile-first | ✅ Met |
| NFR-USE-02 | Navigasi intuitif dan konsisten | Max 3 clicks | ✅ Met |
| NFR-USE-03 | Feedback visual untuk aksi pengguna | Toast/alert | ✅ Met |
| NFR-USE-04 | Support browser modern | Chrome, Firefox, Safari, Edge | ✅ Met |

### Reliability (NFR-REL)
| **ID** | **Kebutuhan** | **Target** | **Status** |
|--------|---------------|------------|------------|
| NFR-REL-01 | Uptime sistem | 99.5% | ✅ Met |
| NFR-REL-02 | Error handling yang proper | Graceful degradation | ✅ Implemented |
| NFR-REL-03 | Custom 404 page | User-friendly | ✅ Implemented |

### Maintainability (NFR-MNT)
| **ID** | **Kebutuhan** | **Implementasi** | **Status** |
|--------|---------------|------------------|------------|
| NFR-MNT-01 | Kode terstruktur dan modular | MVC-like pattern | ✅ Met |
| NFR-MNT-02 | Dokumentasi kode | PHPDoc comments | ✅ Met |
| NFR-MNT-03 | Konfigurasi terpisah dari kode | config/ folder | ✅ Met |

## 4.3 Diagram Pendukung

### 4.3.1 Use Case Diagram
