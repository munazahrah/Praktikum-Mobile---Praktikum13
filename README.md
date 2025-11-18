# Praktikum 13

Project Modul 13 - Operasi CRUD dengan REST API

📖 Deskripsi

Project ini adalah simulasi lengkap pengelolaan data. Anda akan membangun aplikasi yang dapat melakukan 4 operasi dasar database (CRUD) yang terhubung ke internet (REST API).

Anda akan menggunakan layanan API publik (biasanya JSONPlaceholder) untuk mensimulasikan proses:

Create: Mengirim data baru ke server (POST).

Read: Menampilkan data dari server (GET).

Update: Mengubah data yang ada di server (PUT).

Delete: Menghapus data dari server (DELETE).

🎯 Tujuan Utama Project

HTTP Methods: Memahami perbedaan dan penggunaan method GET, POST, PUT, dan DELETE.

Interaksi API: Menggunakan package http untuk berkomunikasi dengan server.

Input User: Menggunakan TextField dalam AlertDialog untuk menerima input data dari pengguna.

Feedback UI: Memberikan umpan balik kepada pengguna (sukses/gagal) menggunakan SnackBar.

State Management: Memperbarui tampilan secara langsung (setState) setelah operasi CRUD berhasil dilakukan.

✅ Daftar Tugas (To-Do List)

Berikut adalah langkah-langkah pengerjaan project ini:

Buat Project & Setup Dependency:

[ ] Buat project baru (misal: crud_flutter_api).

[ ] Tambahkan package http di pubspec.yaml.

[ ] (Opsional) Tambahkan intl dan google_fonts sesuai panduan modul untuk mempercantik UI.

Siapkan Struktur Data (Model):

[ ] Siapkan variabel/model untuk menampung data "Post" (biasanya terdiri dari id, title, body, userId).

Implementasi Fungsi Logika (Logic):

[ ] Fungsi createPost(): Gunakan http.post. Kirim data JSON (title & body) ke API. Jika sukses, tampilkan SnackBar dan update UI.

[ ] Fungsi updatePost(): Gunakan http.put. Kirim data revisi ke URL yang spesifik (berdasarkan ID). Update UI dengan data baru.

[ ] Fungsi deletePost(): Gunakan http.delete. Hapus data berdasarkan ID. Kosongkan tampilan data di UI jika sukses.

Bangun Antarmuka (UI):

[ ] Tampilan Data: Gunakan widget Card untuk menampilkan data (Title & Body) yang sedang aktif/berhasil dibuat.

[ ] Tombol Tambah: Buat FloatingActionButton yang memunculkan Dialog.

[ ] Dialog Input: Buat AlertDialog yang berisi dua TextField (untuk Judul dan Isi) dan tombol "Simpan". Dialog ini digunakan untuk fungsi Create dan Update.

[ ] Tombol Aksi (Edit/Hapus): Di dalam Card, tambahkan tombol/icon untuk memicu fungsi Update dan Delete.

Integrasi & Feedback:

[ ] Hubungkan tombol "Simpan" di dialog dengan fungsi createPost atau updatePost.

[ ] Hubungkan tombol "Hapus" dengan dialog konfirmasi, lalu panggil deletePost.

[ ] PENTING: Pastikan setiap kali operasi berhasil, muncul notifikasi SnackBar (misal warna hijau untuk sukses, merah untuk gagal).
