# Analisis Kompleksitas Algoritma Rekursif dan Iteratif
---
## Implementasi 0/1 Knapsack Problem

### 📘 Deskripsi Proyek

Repository ini berisi implementasi dan analisis perbandingan **algoritma rekursif** dan **algoritma iteratif (Dynamic Programming)** dalam menyelesaikan **0/1 Knapsack Problem**.

Penelitian ini bertujuan untuk membandingkan efisiensi algoritma dari kedua pendekatan tersebut, khususnya dari sisi **kompleksitas waktu dan performa eksekusi**, baik secara **teoretis (Big-O)** maupun secara **empiris** melalui pengujian waktu eksekusi.

Aplikasi dikembangkan untuk mensimulasikan proses optimasi pemuatan barang, di mana pengguna dapat menentukan jumlah barang, bobot, nilai, dan kapasitas knapsack. Sistem kemudian menampilkan hasil nilai maksimum serta waktu eksekusi dari masing-masing algoritma.

---

### 🎯 Tujuan

1. Mengimplementasikan algoritma rekursif dan algoritma iteratif (*Dynamic Programming*) untuk menyelesaikan 0/1 Knapsack Problem.
2. Menganalisis kompleksitas waktu dari kedua algoritma secara teoretis menggunakan notasi **Big-O**.
3. Membandingkan waktu eksekusi berdasarkan hasil pengujian nyata.
4. Menentukan algoritma yang lebih efisien untuk permasalahan optimasi skala besar.

---

### 📐 Konsep 0/1 Knapsack Problem

Setiap barang hanya memiliki dua kemungkinan keputusan: **diambil (1)** atau **tidak diambil (0)**. Tujuan utamanya adalah memaksimalkan total nilai tanpa melebihi kapasitas maksimum.

---

### ⚙️ Implementasi Algoritma

#### 🔂 Algoritma Rekursif (Brute Force)
Bekerja dengan mengevaluasi seluruh kemungkinan kombinasi barang secara berulang.
* **Kompleksitas Waktu:** $O(2^n)$
* **Kompleksitas Ruang:** $O(n)$

#### 🔁 Algoritma Iteratif (Dynamic Programming)
Menggunakan pendekatan *bottom-up* dengan tabel dua dimensi untuk menghindari perhitungan berulang.
* **Kompleksitas Waktu:** $O(n \times W)$
* **Kompleksitas Ruang:** $O(n \times W)$

---

### ✅ Kesimpulan

Berdasarkan analisis, **Algoritma Iteratif (Dynamic Programming)** memiliki efisiensi yang jauh lebih baik dan stabil dibandingkan algoritma rekursif, terutama saat menangani jumlah barang yang besar.
