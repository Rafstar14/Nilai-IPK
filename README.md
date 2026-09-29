Sistem Konversi Nilai & IPK (C++)
Program CLI (Command Line Interface) berbasis C++ yang berfungsi untuk mengonversi nilai angka (skala 0–100) menjadi *Huruf Mutu*, *Sebutan Mutu*, dan *Angka Mutu* secara otomatis berdasarkan standar penilaian akademis.

📌 Fitur Utama
- *Konversi Nilai Otomatis*: Memetakan nilai angka ke dalam rentang mutu akademis.
- *Validasi Input Rigorus*: 
  - Mencegah *crash* jika pengguna memasukkan karakter/huruf alih-alih angka.
  - Memastikan nilai yang dimasukkan berada dalam rentang valid (0 hingga <100).
- *Pengulangan*: Pengguna dapat melakukan perhitungan berulang kali tanpa perlu menjalankan ulang program

⚙️ Penjelasan Kode

1. **Struktur Data (`struct Grade`)**: Mengelompokkan atribut standar mutu (`Nilai`, `huruf`, `sebutan`, dan `angka`) ke dalam satu tipe data terstruktur.
2. **Pencarian Rentang Mutu**: Array `tabel[]` disusun dari nilai tertinggi ke terendah. Program melakukan pencarian sekuensial (*looping*) dan langsung berhenti saat rentang nilai pengguna terpenuhi (`break`).
3. **Pembersihan Buffer Input**: Menggunakan `cin.clear()` dan `cin.ignore()` untuk mengosongkan *stream input* ketika terjadi kegagalan pembacaan tipe data angka.

Cara Menjalankan Program
Prasyarat
Pastikan Anda sudah menginstal kompilator C++ (seperti `g++` atau MinGW) di perangkat Anda.

Langkah-langkah
1. **Clone repositori ini:**
   ```bash
   git clone [https://github.com/Rafstar14/Nilai-IPK.git](https://github.com/Rafstar14/Nilai-IPK.git)
   cd Nilai-IPK

Kompilasi kode program
  ```bash
  g++ code -o konversi_nilai
```

Jalankan Program
```bash
  g++ code -o konversi_nilai
