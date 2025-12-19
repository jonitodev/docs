# BAB VI  
# DOKUMEN HASIL PENGUJIAN

## 6.1 Tujuan Pengujian

Pengujian dilakukan untuk memastikan bahwa seluruh logika internal sistem **Website NCS Laboratory** berjalan sesuai dengan perancangan dan spesifikasi kebutuhan perangkat lunak. Pengujian ini bertujuan untuk mengidentifikasi kesalahan logika, memastikan alur program berjalan dengan benar, serta menjamin kualitas dan keandalan sistem sebelum digunakan secara penuh.

Fokus pengujian pada bab ini adalah **White Box Testing**, yaitu metode pengujian yang dilakukan dengan memahami struktur internal kode program.

Tujuan pengujian meliputi:
1. Memastikan setiap fungsi dan prosedur berjalan sesuai alur logika
2. Menguji percabangan dan perulangan dalam program
3. Memastikan validasi data dan proses bisnis berjalan dengan benar
4. Mengidentifikasi potensi kesalahan logika pada sistem
5. Menjamin kestabilan sistem pada berbagai kondisi input

---

## 6.2 Metode Pengujian

### 6.2.1 White Box Testing

White Box Testing merupakan metode pengujian yang berfokus pada struktur internal dan logika program. Pada metode ini, penguji memahami alur kode sumber dan melakukan pengujian terhadap setiap fungsi utama yang ada di dalam sistem.

Pengujian dilakukan dengan cara:
- Menelusuri kode sumber secara langsung
- Menguji setiap fungsi menggunakan data uji tertentu
- Memastikan setiap jalur eksekusi program telah dijalankan
- Mengevaluasi hasil keluaran sesuai dengan yang diharapkan

---

## 6.3 Teknik White Box Testing yang Digunakan

Teknik White Box Testing yang diterapkan pada proyek ini meliputi:

1. **Statement Coverage**  
   Pengujian dilakukan untuk memastikan setiap baris kode dieksekusi minimal satu kali selama proses pengujian.

2. **Decision Coverage**  
   Pengujian dilakukan pada setiap kondisi logika (if–else) untuk memastikan kondisi benar dan salah dapat dieksekusi dengan baik.

3. **Path Coverage**  
   Pengujian dilakukan untuk memastikan seluruh jalur eksekusi program telah diuji.

4. **Loop Testing**  
   Pengujian dilakukan pada struktur perulangan untuk memastikan perulangan berjalan dengan benar pada kondisi awal, tengah, dan akhir.

---

## 6.4 Lingkungan Pengujian

Pengujian sistem dilakukan pada lingkungan sebagai berikut:

- **Bahasa Pemrograman:** PHP 8.x  
- **Database:** PostgreSQL  
- **Web Server:** Apache / Nginx (dikelola melalui aaPanel)  
- **Sistem Operasi:** Linux (VPS)  
- **Browser:** Google Chrome dan Mozilla Firefox  

Lingkungan pengujian disesuaikan dengan lingkungan produksi agar hasil pengujian mencerminkan kondisi sistem sebenarnya.

---

## 6.5 Skenario Pengujian White Box

Pengujian White Box difokuskan pada modul-modul utama sistem sebagai berikut:
- Modul Autentikasi
- Modul Manajemen Dokumen
- Modul Manajemen Galeri
- Modul Manajemen Agenda
- Modul Pengelolaan Pesan Pengunjung

---

## 6.6 Hasil Pengujian White Box

### 6.6.1 Pengujian Modul Autentikasi

| **No** | **Fungsi yang Diuji** | **Skenario Pengujian** | **Hasil yang Diharapkan** | **Hasil Pengujian** | **Status** |
|------|----------------------|------------------------|---------------------------|---------------------|------------|
| 1 | validasiLogin() | Username dan password valid | Login berhasil | Sesuai | Lulus |
| 2 | validasiLogin() | Password salah | Login ditolak | Sesuai | Lulus |
| 3 | validasiLogin() | Input kosong | Validasi gagal | Sesuai | Lulus |

### 6.6.2 Pengujian Modul Manajemen Dokumen

| **No** | **Fungsi yang Diuji** | **Skenario Pengujian** | **Hasil yang Diharapkan** | **Hasil Pengujian** | **Status** |
|------|----------------------|------------------------|---------------------------|---------------------|------------|
| 1 | uploadDocument() | File PDF valid | File tersimpan | Sesuai | Lulus |
| 2 | uploadDocument() | File non-PDF | Upload ditolak | Sesuai | Lulus |
| 3 | deleteDocument() | Hapus data valid | Data terhapus | Sesuai | Lulus |

### 6.6.3 Pengujian Modul Manajemen Galeri

| **No** | **Fungsi yang Diuji** | **Skenario Pengujian** | **Hasil yang Diharapkan** | **Hasil Pengujian** | **Status** |
|------|----------------------|------------------------|---------------------------|---------------------|------------|
| 1 | uploadGallery() | Upload gambar valid | Gambar tersimpan | Sesuai | Lulus |
| 2 | uploadGallery() | Format tidak valid | Upload ditolak | Sesuai | Lulus |

### 6.6.4 Pengujian Modul Agenda

| **No** | **Fungsi yang Diuji** | **Skenario Pengujian** | **Hasil yang Diharapkan** | **Hasil Pengujian** | **Status** |
|------|----------------------|------------------------|---------------------------|---------------------|------------|
| 1 | createAgenda() | Data agenda valid | Agenda tersimpan | Sesuai | Lulus |
| 2 | updateAgenda() | Edit data agenda | Data terupdate | Sesuai | Lulus |

---

## 6.7 Evaluasi Hasil Pengujian

Berdasarkan hasil pengujian White Box yang telah dilakukan, seluruh fungsi utama sistem telah berjalan sesuai dengan perancangan. Tidak ditemukan kesalahan logika kritis yang dapat mengganggu proses utama sistem.

Seluruh jalur eksekusi program telah diuji dan menghasilkan keluaran yang sesuai dengan hasil yang diharapkan.

---

## 6.8 Kesimpulan Pengujian

Berdasarkan hasil White Box Testing yang dilakukan, dapat disimpulkan bahwa:
1. Struktur logika program telah berjalan dengan baik
2. Seluruh fungsi utama sistem berfungsi sesuai rancangan
3. Sistem siap digunakan dan dilanjutkan ke tahap deployment
4. Tidak ditemukan error kritis pada proses pengujian internal

Dengan demikian, **Website NCS Laboratory** dinyatakan **layak untuk digunakan** sesuai dengan tujuan pengembangan sistem.
