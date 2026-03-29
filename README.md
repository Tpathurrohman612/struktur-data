# STRUKTUR DATA

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white) ![VS Code](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white) ![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

Repository ini berisi kumpulan tugas praktikum untuk mata kuliah **STRUKTUR DATA**. Project ini mendemonstrasikan progresi pembelajaran bahasa pemrograman Java mulai dari implementasi cara deklarasi Tipe Data sampai dengan implementasi metode pencarian sebuah data yang dinamis.

---

## 📁 Struktur Direktori

Penyusunan folder secara standar pada _workspace_ ini meliputi:

- `src/`: Merupakan folder utama yang memuat seluruh baris kode sumber (source code) Java.
- `bin/`: Direktori tempat hasil kompilasi _bytecode_ (file `.class`) secara default dihasilkan oleh compiler.
- `lib/`: Digunakan untuk menyimpan dependensi tambahan jika diperlukan.

---

## 📝 Rincian & Penjelasan Tugas

Kode sumber terbagi menjadi tiga bagian tugas utama yang masing-masing mendemonstrasikan fondasi struktur data, algoritma pengurutan (_sorting_), dan algoritma pencarian (_searching_).

### Tugas 1: Dasar Variabel dan Koleksi Data (`Tugas1.java`)

Berkas ini bertugas sebagai representasi cara inisialisasi dan deklarasi tipe data koleksi di dalam Java. Cakupan pembahasannya meliputi:

- **Variabel Primitif:** Pendeklarasian tipe data integer bernilai `200` dan tipe data String yang berisi kata `"struktur"`.
- **Array Satu Dimensi:** Pendeklarasian himpunan variabel dalam satu baris indeks dengan angka `(12, 10, 40)`.
- **Array Dua Dimensi (Matriks):** Implementasi array multidimensi dalam bentuk matriks 3x3 bersarang yang berisi elemen `{{12,10,40}, {13,11,41}, {14,12,42}}`.
- **Linked List:** Menggunakan _class_ bawaan `java.util.LinkedList` untuk menyimpan rangkaian angka dinamis yaitu `(10, 20, 30, 40, 50)` secara berurutan.

### Tugas 2: Algoritma Pengurutan / Sorting

Berfokus pada pengolahan _array_ tidak beraturan menjadi terurut dari yang paling kecil ke paling besar.

- **Merge Sort (`mergesort.java`):** Mengurutkan himpunan angka berupa `(67, 21, 75, 87, 33, 1)`. Algoritma dipecah menjadi fungsi pembagi nilai tengah `sort()` dan fungsi penggabung nilai `merge()` (metode _Divide and Conquer_).
- **Counting Sort (`countingsort.java`):** Digunakan untuk mengurutkan himpunan tipe data karakter tunggal (`char`) yang bernilai `('w', 'k', 'p', 'a', 'l', 'o')`. Proses ini mengevaluasi jumlah kemunculan elemen dan menempatkannya menggunakan array `output` dan array `count` berukuran 256 byte.

### Tugas 3: Algoritma Pencarian / Searching

Berfokus pada metode pencarian sebuah data yang dinamis diinput langsung oleh pengguna. Kedua program ini telah disematkan `Scanner` untuk memfasilitasi _input_ melalui terminal.

- **Sequential Search (`SequentialSearch.java`):** Memproses pencarian data secara linear / _brute force_. Metode ini digunakan pada susunan array yang **belum terurut** berisi nilai `(65, 21, 43, 76, 121)`. Iterasi dilakukan satu per satu dari elemen paling pertama hingga paling akhir sampai angka kecocokan didapatkan.
- **Binary Search (`BinarySearch.java`):** Algoritma spesifik yang hanya efektif memproses susunan array yang **sudah terurut** secara _ascending_, dalam hal ini menggunakan data `(5, 15, 25, 35, 45)`. Pencarian dilakukan secara rekursif melalui identifikasi variabel batas bawah (`left`), nilai potong tengah (`mid`), dan batas atas (`right`) secara dinamis untuk menyaring blok data yang harus dieliminasi hingga angka incaran berhasil ditemukan pada sebuah _index_.

---

## 🛠️ Teknologi yang Digunakan

- **Bahasa Pemrograman:** Java
- **IDE/Editor:** Visual Studio Code
- **Java Depelopment Kits (JDK):** 21

---
