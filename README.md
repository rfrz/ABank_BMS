# 🏦 Bank Management System (BMS)

**Aplikasi Manajemen Perbankan Berbasis Desktop**

Proyek ini adalah aplikasi desktop sederhana yang dibangun menggunakan **Java** (NetBeans) untuk mensimulasikan sistem operasional bank. Aplikasi ini memungkinkan pengguna untuk membuat akun, melakukan transaksi, dan mengelola profil nasabah, serta dilengkapi dengan fitur login untuk keamanan.

## 📖 Deskripsi Proyek

Aplikasi ini dirancang untuk memudahkan manajemen data nasabah dan transaksi perbankan. Menggunakan antarmuka grafis (GUI) yang dibangun dengan Java Swing, aplikasi ini menawarkan pengalaman pengguna yang interaktif. Data nasabah dan transaksi disimpan secara lokal menggunakan database **SQLite**.

### ✨ Fitur Utama

* **Autentikasi Aman:** Halaman Login dan Register untuk nasabah.
* **Manajemen Akun:** Pembuatan akun baru dengan data lengkap (Nama, Tgl Lahir, Alamat, dll).
* **Dashboard Nasabah (`MyPage`):**
    * Cek Saldo (Balance Enquiry).
    * Transfer Dana.
    * Setor Tunai (Deposit) & Tarik Tunai (Withdraw).
    * Riwayat Transaksi.
    * Edit Profil.
* **Admin Panel:** Fitur khusus untuk administrator mengelola data user (jika diaktifkan).
* **Splash Screen:** Tampilan loading awal yang interaktif.

---

## 🛠️ Tech Stack & Dependencies

Proyek ini dibangun menggunakan teknologi dan pustaka berikut:

* **Bahasa Pemrograman:** Java (JDK 8+)
* **IDE:** NetBeans IDE (Direkomendasikan)
* **Database:** SQLite (`bank.db` / `bank1.db`)
* **GUI Framework:** Java Swing & AWT
* **External Libraries (JARs):**
    * `sqlite-jdbc`: Driver koneksi ke database SQLite.
    * `rs2xml`: Untuk menampilkan data database ke tabel GUI (JTable).
    * `jcalendar`: Widget kalender untuk input tanggal.
    * `JTattoo`: Library Look-and-Feel untuk mempercantik tampilan aplikasi.

---

## 📂 Struktur Project

Berikut adalah gambaran singkat struktur folder penting dalam repo ini:

* **`src/`**: Berisi seluruh source code Java (`.java`) dan desain form (`.form`).
    * `Loading.java`: Entry point aplikasi (Splash screen).
    * `Authentication.java`: Halaman Login.
    * `Account.java`: Form pendaftaran akun baru.
    * `MyPage.java`: Halaman utama transaksi nasabah.
    * `javaconnect.java`: Modul koneksi ke database SQLite.
    * `img/` (atau root src): Aset gambar seperti `IBanking.png`, ikon kunci, dll.
* **`*.jar`**: File library pendukung yang wajib ditambahkan ke classpath.
* **`bank.db`**: File database utama.

---

## 🚀 Cara Menjalankan (Setup)

Ikuti langkah-langkah ini untuk menjalankan aplikasi di komputer lokal:

### 1. Prasyarat
Pastikan komputer kamu sudah terinstall:
* Java Development Kit (JDK)
* NetBeans IDE (atau IDE Java lain seperti IntelliJ/Eclipse)

### 2. Import Project
1.  Buka NetBeans IDE.
2.  Pilih **File** > **Open Project**.
3.  Arahkan ke folder tempat kamu menyimpan repo ini (`ABank_BMS`).

### 3. Konfigurasi Library
Agar aplikasi berjalan tanpa error, kamu harus memastikan semua file `.jar` terhubung:
1.  Klik kanan pada nama project di panel kiri -> **Properties**.
2.  Pilih menu **Libraries**.
3.  Jika ada library yang merah/missing, hapus dan tambahkan kembali file `.jar` yang ada di root folder repo ini:
    * `sqlite-jdbc-3.27.2.1.jar`
    * `rs2xml.jar`
    * `jcalendar-1.4.jar`
    * `JTattoo-1.6.13.jar`

### 4. Jalankan Aplikasi
1.  Cari file **`Loading.java`** di dalam package `src`.
2.  Klik kanan file tersebut dan pilih **Run File** (Shift+F6).
3.  Tunggu loading selesai, dan aplikasi siap digunakan!

---

## 📸 Tampilan Aplikasi (Preview)

Aplikasi ini menggunakan tema dari **JTattoo** untuk tampilan yang lebih modern, serta dilengkapi dengan ikon-ikon intuitif untuk setiap menu transaksi.

> *Catatan: Pastikan file `bank.db` berada di direktori root project saat aplikasi dijalankan agar koneksi database berhasil.*

---

**👨‍💻 Author**
* **Dibuat oleh:** rfrz, rusdi, rafi, ojan
