#ANALISIS PERBANDINGAN EFISIENSI ALGORITMA REKURSIF DAN ITERATIF (DYNAMIC PROGRAMMING) DALAM OPTIMASI PEMUATAN BARANG (0/1 KNAPSACK PROBLEM)

#Deskripsi Proyek
Repository ini berisi implementasi dan analisis perbandingan algoritma rekursif dan algoritma iteratif (Dynamic Programming) dalam menyelesaikan 0/1 Knapsack Problem.

Penelitian ini bertujuan untuk membandingkan efisiensi algoritma dari kedua pendekatan tersebut, khususnya dari sisi kompleksitas waktu dan performa eksekusi, baik secara teoretis menggunakan notasi Big-O maupun secara empiris melalui pengujian waktu eksekusi.

Aplikasi dikembangkan untuk mensimulasikan proses optimasi pemuatan barang, di mana pengguna dapat menentukan jumlah barang, bobot, nilai, dan kapasitas knapsack. Sistem kemudian menampilkan hasil nilai maksimum yang dapat diperoleh serta waktu eksekusi dari masing-masing algoritma.


#🎯Tujuan
1. Mengimplementasikan algoritma rekursif dan algoritma iteratif (Dynamic Programming) untuk menyelesaikan 0/1 Knapsack Problem.
2. Menganalisis kompleksitas waktu dari kedua algoritma secara teoretis menggunakan notasi Big-O.
3. Membandingkan waktu eksekusi algoritma rekursif dan iteratif berdasarkan hasil pengujian.
4. Menentukan algoritma yang lebih efisien dan tepat digunakan untuk permasalahan optimasi pemuatan barang.

#📐 Konsep 0/1 Knapsack Problem
0/1 Knapsack Problem merupakan permasalahan optimasi klasik di mana setiap barang hanya memiliki dua kemungkinan keputusan, yaitu diambil (1) atau tidak diambil (0).
Setiap barang memiliki:
  1. Berat (weight)
  2. Nilai (value)
Tujuan utama dari permasalahan ini adalah memaksimalkan total nilai barang yang dimasukkan ke dalam knapsack tanpa melebihi kapasitas maksimum yang tersedia.

#⚙️ Implementasi Algoritma
#🔂 Algoritma Rekursif (Brute Force)
Algoritma rekursif bekerja dengan mengevaluasi seluruh kemungkinan kombinasi barang yang dapat dimasukkan ke dalam knapsack. Untuk setiap barang, algoritma mempertimbangkan dua pilihan, yaitu mengambil atau tidak mengambil barang tersebut, kemudian memanggil dirinya sendiri untuk menyelesaikan sub-permasalahan.
Karakteristik:
  1. Menggunakan pemanggilan fungsi berulang (rekursi)
  2. Mengevaluasi semua kemungkinan solusi
Kompleksitas:
  1. Kompleksitas waktu: O(2ⁿ)
  2. Kompleksitas ruang: O(n)
Algoritma ini sederhana secara konsep, namun tidak efisien untuk jumlah barang yang besar karena pertumbuhan waktu eksekusi yang sangat cepat.
#🔁 Algoritma Iteratif (Dynamic Programming)
Algoritma iteratif menggunakan pendekatan Dynamic Programming dengan membangun tabel dua dimensi untuk menyimpan hasil perhitungan sub-masalah. Pendekatan ini menghindari perhitungan berulang dengan menyimpan hasil sementara dan membangunnya secara bottom-up.
Karakteristik:
  1. Menggunakan struktur perulangan
  2. Setiap sub-masalah dihitung satu kali
Kompleksitas:
  1. Kompleksitas waktu: O(n × W)
  2. Kompleksitas ruang: O(n × W)
Algoritma ini lebih efisien dan stabil dibandingkan algoritma rekursif, terutama untuk jumlah barang yang besar.
