# Laporan Modul 1: Perkenalan Laravel
**Mata Kuliah:** Workshop Web Lanjut   
**Nama:** [TM IRSAN TRIFIERY]  
**NIM:** [2024573010112]  
**Kelas:** [TI-2B]  

---

## Abstrak 
Laporan Praktikum Mengenal apa itu laravel, komponen bawaan laravel, dan Instalasi Ekosistem Laravel.

---

## 1. Pendahuluan
- Apa itu Laravel?
Laravel adalah framework web PHP yang populer, bersifat open-source, dan dirancang untuk membangun aplikasi web modern yang skalabel dan aman.
Laravel merupakan framework high-level yang bersifat opinionated (punya aturan dan konvensi tertentu).

- Karakteristik utama (MVC, opinionated, dsb.)
 Arsitektur MVC → memisahkan Model, View, dan Controller agar kode lebih terstruktur.
 Opinionated Framework → menyediakan aturan dan standar bawaan yang memandu developer.
 Routing yang sederhana → mudah dalam mengatur URL dan request.
 ORM (Eloquent) → mempermudah interaksi dengan database menggunakan model berbasis objek.
 Fitur lengkap → sudah ada autentikasi, middleware, queue, session, mail, dan lainnya.

- Untuk jenis aplikasi apa Laravel cocok?
 Laravel cocok digunakan untuk membangun:
  Aplikasi web berskala kecil hingga besar.
  Sistem manajemen (misalnya e-commerce, CMS, dashboard).
  API backend untuk aplikasi mobile atau web modern.
---

## 2. Komponen Utama Laravel (ringkas)
Tuliskan penjelasan singkat (1–3 kalimat) untuk tiap komponen berikut:

 Blade → templating engine untuk tampilan dinamis.
 Eloquent → ORM untuk interaksi database pakai model.
 Routing → atur URL dan arahkan request.
 Controllers → logika aplikasi, penghubung model & view.
 Migrations & Seeders → kelola struktur & isi data awal database.
 Artisan CLI → tool command line untuk otomatisasi.
 Testing (PHPUnit) → uji aplikasi agar bebas bug.

---

## 3. Berikan penjelasan untuk setiap folder dan files yang ada didalam struktur sebuah project laravel.
FOLDER:

App
Folder app berisi kode-kode inti dari aplikasi seperti Model, Controller, Commands, Listener, Events, dll. Poinnya, hampir semua class dari aplikasi berada di folder ini.

Bootstrap
Folder bootstrap berisi file app.php yang dimana akan dipakai oleh Laravel untuk boot setiap kali dijalankan.

Config
Folder config seperti namanya, berisi semua file konfigurasi aplikasi Anda.

Database
Folder database berisi database migrations, model factories, dan seeds. Folder ini akan bertanggung jawab dengan pembuatan dan pengisian tabel-tabel database.

Public
Folder public memiliki file index.php yaitu entry point dari semua requests yang masuk/diterima ke aplikasi. Folder ini juga tempat menampung gambar, Javascript, dan CSS.

Resources
Folder resources berisi semua route yang disediakan aplikasi. Sebagai default, beberapa file routing akan tersedia seperti: web.php, api.php, console.php, dan channels.php. Folder ini adalah tempat dimana kita memberikan koleksi definisi route aplikasi.

Storage
Folder storage adalah tempat dimana cache, logs, dan file sistem yang ter-compile hidup.

Tests
Folder tests adalah tempat dimana unit dan integration tests tinggal.

Vendor
Folder vendor adalah dimana tempat folder-folder dependencies third-party yang telah di-install oleh composer berada.



FILES:
.editorconfig
Berguna untuk memberi IDE/text editor instruksi tentang standar coding Laravel seperti whitespace, besar identasi, dll.

.env dan .env.example
Tempat dimana variable environment aplikasi ditempatkan (variabel yang diekspektasikan akan berbeda di setiap sistem) seperti nama database, username database, password database. 

.gitignore dan .gitattributes
File konfigurasi git.

artisan
Memungkinkan anda untuk menjalankan perintah artisan dari command line.

composer.json dan composer.lock 
File konfigurasi untuk composer. File ini adalah informasi dasar tentang projek dan juga mendefinisikan dependencies yang digunakan.

package.json
Mirip-mirip dengan composer.json tapi untuk aset-aset dan dependencies front-end.

phpunit.xml
Sebuah file konfigurasi untuk PHPUnit, tools yang digunakan Laravel untuk testing.

readme.md
Sebuah markdown file yang memberikan pengenalan dasar tentang Laravel.


---

## 4. Diagram MVC dan Cara kerjanya

> Letakkan gambar di dalam folder `laporan1/gambar/`. Kemudian masukkan gambar tersebut ke laporan. 

lihat cara nya disini https://www.ulas.in/komputer/markdown-memasukkan-gambar/

![Diagram MVC](./gambar/Diagram%20MVC.jpg)

CARA KERJA :  Proses pertama adalah view akan meminta data untuk ditampilkan dalam bentuk grafis kepada pengguna.
              Permintaan tersebut diterima oleh controller dan diteruskan ke model untuk diproses.
              Model akan mencari dan mengolah data yang diminta di dalam database
              Setelah data ditemukan dan diolah, model akan mengirimkan data tersebut kepada controller untuk ditampilkan di view.
              Controller akan mengambil data hasil pengolahan model dan mengaturnya di bagian view untuk ditampilkan kepada pengguna.

---

## 6. Kelebihan & Kekurangan (refleksi singkat)
- Kelebihan Laravel menurut Anda
    memiliki banyak fitur bawaan, ORM untuk database, Artisan CLI, serta dukungan komunitas besar sehingga memudahkan dan mempercepat pengembangan aplikasi web.
    
- Hal yang mungkin menjadi tantangan bagi pemula
    Instalasi & konfigurasi awal (Composer, PHP, database, environment).
    Memahami konsep MVC dan alur kerja Laravel.
    Routing & Controller yang awalnya terasa membingungkan.
---

## 7. Referensi
Cantumkan sumber yang Anda baca (buku, artikel, dokumentasi) — minimal 2 sumber. Gunakan format sederhana (judul — URL).

Penjelasan tiap folder dan file dalam struktur project laravel - https://www.barajacoding.or.id/mengenal-struktur-folder-dan-file-pada-laravel/

Penjelasan Diagram dan cara kerja MVC - https://www.dicoding.com/blog/apa-itu-mvc-pahami-konsepnya/


---
