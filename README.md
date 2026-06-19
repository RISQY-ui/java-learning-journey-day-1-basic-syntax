# java-learning-journey-day-1-basic-syntax
Learning Java basics step by step using Termux. Starting from print output and loop fundamentals.

# Panduan Lengkap Java di Termux

**Dokumentasi Teknis** | **Platform: Android (Termux)** | **Tanggal: 19 Juni 2026**

---

## 📋 Daftar Isi

- [1. Pendahuluan](#1-pendahuluan)
- [2. Instalasi Java di Termux](#2-instalasi-java-di-termux)
- [3. Membuat File Java Pertama](#3-membuat-file-java-pertama)
- [4. Struktur Dasar Java](#4-struktur-dasar-java)
- [5. Compile & Jalankan Program](#5-compile--jalankan-program)
- [6. Contoh Program (Perulangan)](#6-contoh-program-perulangan)
- [7. Error Paling Sering Terjadi](#7-error-paling-sering-terjadi)
- [8. Pola Dasar Java yang Harus Diingat](#8-pola-dasar-java-yang-harus-diingat)
- [9. Alur Cepat di Termux](#9-alur-cepat-di-termux)
- [10. Level Berikutnya](#10-level-berikutnya)

---

## 1. Pendahuluan

### Apa itu Java?

Java adalah bahasa pemrograman yang **populer**, **stabil**, dan **banyak digunakan** di dunia enterprise, aplikasi Android, hingga backend development.

### Mengapa Belajar Java di Termux?

| Keuntungan | Keterangan |
|------------|-------------|
| **Tanpa Laptop** | Bisa belajar Java langsung dari HP |
| **Portabel** | Bawa kemanapun, praktik kapanpun |
| **Ringan** | Termux + OpenJDK 21 tidak memberatkan HP |
| **Lengkap** | Bisa compile, run, bahkan bikin project kecil |

---

## 2. Instalasi Java di Termux

### Langkah 1: Update & Upgrade

```bash
pkg update && pkg upgrade
```

Langkah 2: Install OpenJDK 21

```bash
pkg install openjdk-21
```

Langkah 3: Verifikasi Instalasi

Cek apakah Java sudah terinstall dengan benar:

```bash
java --version
javac --version
```

Hasil yang Diharapkan:

Perintah Output Contoh
java --version openjdk version "21.0.x"
javac --version javac 21.0.x

✅ Jika kedua perintah di atas menampilkan versi, maka Java sudah siap digunakan.

---

3. Membuat File Java Pertama

Langkah 1: Buka Editor di Termux

```bash
nano Main.java
```

Langkah 2: Ketik Kode Java

Ketik kode berikut (penjelasan ada di bagian selanjutnya).

Langkah 3: Simpan File

Tombol Fungsi
CTRL + O Menyimpan file
Enter Konfirmasi nama file
CTRL + X Keluar dari editor nano

---

4. Struktur Dasar Java (WAJIB)

Kode Dasar

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Halo Faris");
    }
}
```

Penjelasan Setiap Bagian

Bagian Kode Fungsi
public class Main Membuat class bernama Main — nama file harus sama dengan nama class!
public static void main(String[] args) Method utama — titik awal semua program Java. Wajib ada!
System.out.println("..."); Perintah mencetak teks ke layar
{ } Menandai blok kode (awal & akhir)
; Mengakhiri setiap perintah

⚠️ Aturan Penting: Nama file .java HARUS SAMA dengan nama class di dalamnya. Contoh: file Main.java → class Main

---

5. Compile & Jalankan Program

Compile (Ubah Kode Menjadi Program)

```bash
javac Main.java
```

Hasil: Jika sukses, akan muncul file baru bernama Main.class (file bytecode Java).

Jalankan Program

```bash
java Main
```

Output:

```
Halo Faris
```

💡 Tips: Jalankan java tanpa .class atau .java — cukup nama class-nya saja.

---

6. Contoh Program (Perulangan)

Kode

```java
public class Main {
    public static void main(String[] args) {
        for (int i = 0; i <= 5; i++) {
            System.out.println(i);
        }
    }
}
```

Output

```
0
1
2
3
4
5
```

Penjelasan

Bagian Kode Fungsi
for (int i = 0; i <= 5; i++) Perulangan dari 0 sampai 5
System.out.println(i); Cetak nilai i setiap iterasi

---

7. Error Paling Sering Terjadi

❌ Salah: Huruf kecil

```java
system.out.println("Halo");
```

✅ Benar: Huruf besar

```java
System.out.println("Halo");
```

📌 Pelajaran: Java adalah case-sensitive — huruf besar dan kecil dibedakan!

Kesalahan Lain yang Sering Muncul

Error Penyebab Solusi
class Main is public, should be declared in a file named Main.java Nama file tidak sama dengan nama class Ganti nama file atau class agar sama
cannot find symbol Ada typo di nama method/variabel Cek kembali penulisan kode
';' expected Lupa tanda titik koma (;) di akhir perintah Tambahkan ;

---

8. Pola Dasar Java yang Harus Diingat

Elemen Contoh Fungsi
class class Main Membungkus semua kode
main method public static void main Titik masuk program
print System.out.println Mencetak ke layar
curly braces { } Membuka & menutup blok kode
semicolon ; Mengakhiri perintah
parentheses ( ) Mengelompokkan parameter

---

9. Alur Cepat di Termux

```bash
# 1. Buat file
nano Main.java

# 2. Compile (ubah jadi program)
javac Main.java

# 3. Jalankan
java Main
```

---

10. Level Berikutnya

Setelah menguasai dasar, Faris akan belajar:

Topik Fungsi
Scanner Menerima input dari keyboard
if-else Percabangan (keputusan)
while loop Perulangan dengan kondisi
array Menyimpan banyak data
method Membuat fungsi sendiri
OOP Object-Oriented Programming (class & object)

---

📊 Ringkasan Perintah

Perintah Fungsi
pkg install openjdk-21 Install Java
java --version Cek versi Java
javac Main.java Compile file Java
java Main Jalankan program
nano Main.java Buat/edit file Java

---

✅ Status Akhir

Komponen Status
Java di Termux ✅ Terinstall (openjdk-21)
File Main.java ✅ Bisa dibuat
Compile javac ✅ Berjalan normal
Run java ✅ Berjalan normal
Program Halo ✅ Output sesuai

---

Panduan Lengkap Java di Termux. Disusun untuk keperluan belajar dan arsip pribadi.
Cocok untuk pemula yang ingin belajar Java langsung dari HP.
