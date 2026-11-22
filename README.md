# Agenda Tugas Siswa (Kotlin Console)

Aplikasi Kotlin Console untuk mencatat dan mengelola tugas sekolah. Proyek ini dibuat untuk Jobsheet 6 Mobile Programming (Git dan GitHub).

## Latar Belakang dan Masalah
Siswa sering lupa tugas yang harus dikerjakan karena pencatatannya tidak teratur. Aplikasi ini membantu siswa menyimpan daftar tugas beserta statusnya dalam satu program sederhana.

## Pengguna dan Tujuan
- **Pengguna:** siswa SMK kelas XI.
- **Tujuan:** mencatat, melihat, mencari, mengubah status, dan menghapus tugas, serta menyimpan data ke berkas agar tidak hilang saat program ditutup.

## Fitur Utama
1. Tambah tugas (validasi ID dan judul tidak kosong, ID tidak boleh duplikat)
2. Tampilkan daftar tugas
3. Cari tugas berdasarkan ID
4. Ubah status tugas (Belum / Selesai)
5. Simpan data ke berkas
6. Hapus tugas (fitur tambahan)

## Teknologi dan Struktur Berkas
- Bahasa: Kotlin (aplikasi console)
- IDE: IntelliJ IDEA
- Version control: Git dan GitHub

```
src/
├── Main.kt            (menu dan alur utama program)
├── Model.kt           (data class Tugas)
├── Penyimpanan.kt     (membaca dan menyimpan data ke berkas)
└── TugasService.kt    (logika tambah, tampil, cari, ubah status, hapus)
agenda_tugas_tp6.txt   (berkas data, dibuat otomatis saat data disimpan)
```

## Cara Menjalankan
1. Clone repository: `git clone https://github.com/JonathanAaronn/TP6_MiniProject_JonathanAaron.git`
2. Buka proyek di IntelliJ IDEA.
3. Buka `src/Main.kt`, lalu klik tombol Run pada fungsi `main`.
4. Pilih menu dengan mengetik angka lalu tekan Enter.

## Contoh Penggunaan atau Output
```
=== AGENDA TUGAS ===
1. Tambah tugas
2. Tampilkan tugas
3. Cari tugas
4. Ubah status
5. Simpan data
6. Hapus tugas
0. Keluar
Pilihan: 1
ID tugas: T01
Judul tugas: Mengerjakan jobsheet Git
Tugas ditambahkan
```

## Hasil Pengujian
Pengujian dilakukan dengan 12 skenario, antara lain mulai tanpa berkas, tambah tugas valid, ID duplikat, judul kosong, cari tugas, ubah status, pilihan menu salah, simpan dan buka ulang, serta berkas rusak. Seluruh skenario berjalan sesuai hasil yang diharapkan.

## Pembagian Tugas dan Branch
- `main`: branch utama berisi program yang sudah teruji.
- `fitur-menu`: pengembangan menu utama aplikasi.
- `fitur-lain`: pengembangan fitur tambahan (pencarian dan hapus tugas).
- Pengembang: Jonathan Aaron Framon.

## Riwayat Pengembangan Ringkas
1. Menyiapkan struktur awal mini project
2. Menambahkan judul, deskripsi, dan nama siswa pada README.md
3. Menambahkan program Kotlin untuk menampilkan nama proyek
4. Memperbaiki tampilan output dengan menambahkan nama pembuat
5. Menambahkan menu utama aplikasi (branch `fitur-menu`)
6. Menambahkan menu pencarian tugas (branch `fitur-lain`)
7. Menambahkan fitur hapus tugas
8. Menggabungkan fitur hapus tugas ke main

## Keterbatasan dan Rencana Pengembangan
- Belum memiliki tampilan grafis (GUI) dan hanya untuk satu pengguna.
- Data disimpan di berkas teks, bukan database.
- Rencana: menambah tenggat dan mata pelajaran pada tugas, filter status, serta pengurutan tugas.