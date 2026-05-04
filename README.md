# 🚀 AI Learning Log: Pandas Foundation

Persiapan PKL AI (Juli 2026). Catatan singkat tentang progres belajar harian.

## 📅 Log: 3 Mei 2026
Hari ini fokus pada setting lingkungan kerja dan dasar pengolahan data menggunakan Pandas.

### ✅ Kesimpulan Pelajaran:
1. **Tooling:** Berhasil migrasi dari Google Colab ke **VS Code** menggunakan ekstensi Jupyter (`.ipynb`) agar lebih *offline-ready*.
2. **Library:** Pandas adalah library wajib AI untuk manipulasi tabel (DataFrame).
3. **Data Creation:** Membuat tabel secara manual menggunakan struktur *Dictionary* Python.
4. **Data Inspection:** - `.info()`: Mengecek kesehatan data (tipe data & baris kosong).
   - `.describe()`: Melihat statistik cepat (rata-rata, min, max) dari data angka.
5. **Data Selection:** Mengambil satu kolom spesifik dari tabel menggunakan indeks label (`df['Nama_Kolom']`).

### 🛠️ Environment:
- Editor: VS Code
- Language: Python 3.14
- Library: Pandas

---
*Next: Data Cleaning & Filtering.*
## 🛠️ Proyek Analisis Data Pelamar AI

Proyek ini mendemonstrasikan alur kerja (workflow) dasar seorang Data Scientist, mulai dari membersihkan data yang kotor hingga menyajikannya dalam bentuk visual.

### 1. 🧹 Data Cleaning (Pembersihan Data)
Data dunia nyata seringkali memiliki nilai kosong (`NaN`). Kami menggunakan teknik **Imputasi** untuk menanganinya tanpa menghapus informasi berharga:
* **Kolom Angka (Skill_Python)**: Menggunakan **Rata-rata (Mean)** agar distribusi data tetap terjaga.
* **Kolom Teks (Kota)**: Menggunakan **Modus (Mode)** atau nilai yang paling sering muncul untuk mengisi kekosongan.



### 2. 🔍 Advanced Filtering (Penyaringan Tingkat Lanjut)
Kami menggunakan operator logika Pandas untuk menemukan kandidat yang paling sesuai dengan kriteria spesifik:
* `&` (**AND**): Semua syarat harus terpenuhi.
* `|` (**OR**): Salah satu syarat terpenuhi sudah cukup.
* `~` (**NOT**): Mengecualikan data tertentu (misal: mencari kandidat di luar kota tertentu).

### 3. 📊 Data Visualization (Visualisasi Data)
Kami membandingkan dua library populer untuk melihat pola data:
* **Matplotlib**: Untuk grafik batang dasar yang cepat.
* **Seaborn**: Untuk grafik yang lebih kaya informasi, menggunakan warna (*hue*) untuk membedakan kategori kota pelamar secara instan.