Nomor Kelompok 53
Data Science Teori IF-E

** Popol Ruby Top BEKASI**
* **Anggota Kelompok:**
  1. 123240184 - Mirza Aditya M   (IF-D) 
  2. 123240194 - Dhimas Naufal F  (IF-B)
  3. 123240207 - Akbar Faqih A    (IF-G)
  4. 123240221 - Adiel Khairullah (IF-E)

# README — Proyek Akhir Praktikum Data Science

## 1. Ringkasan Proyek

**Judul:** Klasifikasi Performa Penjualan Produk Fashion untuk Mendukung Pengambilan Keputusan Bisnis Retail menggunakan Algoritma Random Forest

Proyek ini mengklasifikasikan performa penjualan produk fashion ke dalam tiga kelas, yaitu **High Sales**, **Medium Sales**, dan **Low Sales**, menggunakan algoritma **Random Forest**. Alur pengerjaan mengikuti tahapan Business Understanding, Data Gathering, EDA, Cleaning dan Preprocessing, Modelling, Evaluasi, serta Konklusi. Seluruh kode, hasil, dan penjelasan tersimpan di dalam `presentasi.ipynb`.

Dataset awal berisi 100.000 baris dan 20 kolom. Setelah melalui proses cleaning (penghapusan 1.368 baris dengan nilai negatif, imputasi median, dan penghapusan outlier dengan aturan IQR) serta pemilihan 17 dari 19 prediktor, model dilatih dengan 100 pohon, `max_depth=5`, dan `criterion='gini'`.

Hasil evaluasi model tercatat dengan accuracy **0,3389** dan macro F1 **0,3145**. Sebagai pembanding, `DummyClassifier` memperoleh accuracy **0,3354** dan macro F1 **0,1674**. Kedua angka ini dibaca bersama hasil EDA yang menunjukkan sebaran fitur di ketiga kelas relatif mirip. 
## 2. Informasi Anggota dan Kontribusi

Seluruh kode di dalam notebook dikerjakan bersama oleh keempat anggota dengan porsi yang sama, mulai dari eksplorasi data, cleaning dan preprocessing, pemodelan, sampai evaluasi. Pembagian pada tabel berikut hanya menunjukkan fokus penulisan penjelasan, bukan pembatasan dalam mengerjakan kode.

| No | NIM | Nama | Kelas | Kontribusi |
|---|---|---|---|---|
| 1 | 123240184 | Mirza Aditya M | IF-D | Ikut menulis dan menjalankan seluruh kode; fokus penjelasan B (Bab 1) dan (Bab 7)|
| 2 | 123240194 | Dhimas Naufal F | IF-B | Ikut menulis dan menjalankan seluruh kode; fokus penjelasan  (Bab 5) dan Cleaning serta  (Bab 3) |
| 3 | 123240207 | Akbar Faqih A | IF-G | Ikut menulis dan menjalankan seluruh kode; fokus penjelasan (Bab 4) dan Evaluasi (Bab 2) |
| 4 | 123240221 | Adiel Khairullah | IF-E | Ikut menulis dan menjalankan seluruh kode; fokus penjelasan (Bab 6) dan README ini, serta mengoordinasikan peninjauan ulang keselarasan seluruh isi notebook. |

Keempat anggota bersama-sama memeriksa keselarasan antara rumusan masalah, hasil eksperimen, dan kesimpulan yang ditulis di notebook.

## 3. Sumber Data

- **Nama dataset:** Dynamic Apparel Sales Dataset with Anomalies
- **Sumber:** Kaggle, oleh rayzem
- **Tautan:** https://www.kaggle.com/datasets/rayzem/dynamic-apparel-sales-dataset-with-anomalies
- **File lokal yang digunakan:** `Multiclass_Clothing_Sales_Dataset.csv` (salinan dataset yang ditempatkan di folder yang sama dengan notebook)
- **Ukuran:** 100.000 baris, 20 kolom
- **Struktur:** 19 kolom prediktor dan 1 kolom target `Sales_Category` dengan tiga kategori, yaitu High Sales, Medium Sales, dan Low Sales
- **Karakteristik:** data mengandung missing value pada lima kolom numerik serta sejumlah anomali, sehingga memerlukan tahap cleaning sebelum pemodelan

Dataset dipilih karena jumlahnya memadai, memiliki fitur kategorikal dan numerik, serta menyediakan label performa penjualan yang sesuai untuk permasalahan klasifikasi multiclass.

### Urutan isi notebook

1. Business Understanding
2. Data Gathering
3. Exploratory Data Analysis
4. Cleaning dan Preprocessing
5. Modelling
6. Evaluasi
7. Konklusi
