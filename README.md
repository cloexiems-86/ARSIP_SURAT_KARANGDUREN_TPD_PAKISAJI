# Aplikasi Pengarsipan Surat Resmi Kelurahan Karangduren

## Deskripsi
Aplikasi ini dikembangkan untuk membantu perangkat desa/kelurahan dalam **menyimpan, mengarsipkan, dan mencari surat-surat resmi** yang sudah diterbitkan.  
Setiap surat yang diterbitkan akan di-scan dalam bentuk PDF lalu diunggah ke sistem. Ketika surat tersebut dibutuhkan kembali, perangkat desa cukup membuka aplikasi, mencari surat berdasarkan judul, dan mengunduh file yang tersimpan.

---

## Tujuan
- Membantu perangkat desa dalam **mengelola arsip surat resmi secara digital**.  
- Mempermudah **pencarian surat** berdasarkan judul/kata kunci.  
- Menyediakan **fitur unggah file PDF** surat hasil scan.  
- Memastikan surat resmi yang sudah disimpan dapat **diakses dan diunduh kembali** kapan saja.  
- Mengurangi risiko kehilangan arsip dan meningkatkan efisiensi kerja perangkat desa.  

---

## Fitur Utama
- **Upload Surat Resmi (PDF):** surat hasil scan dapat disimpan ke sistem.  
- **Pencarian Surat:** cari surat berdasarkan judul atau kata kunci.  
- **Download Surat:** surat yang sudah tersimpan dapat diunduh kembali.  
- **Manajemen Arsip:** lihat daftar semua surat resmi yang sudah diunggah.  
- **User Management (opsional):** pengaturan hak akses admin/petugas.  

---

## Persyaratan Sistem
- PHP >= 8.0  
- MySQL / MariaDB  
- Web server (XAMPP, Laragon, atau PHP built-in server)  
- Composer (jika menggunakan framework Laravel)  
- Node.js & npm (jika menggunakan Laravel Mix/Vite untuk asset build)  

---

## Instalasi
1. Clone repository:
   ```bash
   git clone https://github.com/username/arsip-surat-kelurahan.git
   cd arsip-surat-kelurahan
   ```

2. Install dependencies (jika menggunakan Laravel):
   ```bash
   composer install
   npm install && npm run dev
   ```

3. Salin file `.env.example` menjadi `.env`, lalu sesuaikan konfigurasi database:
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. Buat database baru di MySQL (contoh: `arsip_surat_lsp`).

5. Import file `database.sql`:
   - Via terminal:
     ```bash
     mysql -u root -p arsip_surat_lsp < database.sql
     ```
   - Via phpMyAdmin: pilih database → Import → pilih file `database.sql`.

6. Jalankan aplikasi:
   - Jika Laravel:
     ```bash
     php artisan serve
     ```
     Akses melalui browser: [http://127.0.0.1:8000](http://127.0.0.1:8000)  
   - Jika tanpa framework: letakkan folder project di `htdocs/` (XAMPP) lalu buka [http://localhost/nama-folder](http://localhost/nama-folder).

---

---

## dokumentasi beberapa halaman 

### Halaman Kategori Surat
![Kategori Surat](https://github.com/user-attachments/assets/3ea4f159-cfc7-4b25-9d69-ee3e0db41e23)

### Halaman About
![About](https://github.com/user-attachments/assets/39185451-2835-45ce-b531-94a0a3d65e68)

### Halaman Dashboard
![Dashboard](https://github.com/user-attachments/assets/2cc892f8-82e1-4e7f-a49e-419918f73c90)

---
