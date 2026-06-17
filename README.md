# 📘 Tutorial HTML dari A-Z untuk Pemula

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Level](https://img.shields.io/badge/Level-Pemula-brightgreen?style=for-the-badge)
![Bahasa](https://img.shields.io/badge/Bahasa-Indonesia-red?style=for-the-badge)

Selamat datang! Tutorial ini akan mengajarkan kamu HTML dari nol sampai bisa membuat halaman web sendiri. Tidak perlu pengalaman coding sebelumnya — kita mulai dari yang paling dasar, lengkap dengan contoh kode yang bisa langsung dipraktikkan.

> 💡 **Cara pakai:** Salin contoh kode ke file `index.html`, lalu buka di browser. Detail langkahnya ada di bagian [Membuat File HTML Pertama](#3-membuat-file-html-pertama).

## 📑 Daftar Isi

1. [Apa itu HTML?](#1-apa-itu-html)
2. [Persiapan Alat](#2-persiapan-alat)
3. [Membuat File HTML Pertama](#3-membuat-file-html-pertama)
4. [Struktur Dasar HTML](#4-struktur-dasar-html)
5. [Tag dan Elemen](#5-tag-dan-elemen)
6. [Heading (Judul)](#6-heading-judul)
7. [Paragraf dan Teks](#7-paragraf-dan-teks)
8. [Format Teks](#8-format-teks)
9. [Link (Tautan)](#9-link-tautan)
10. [Gambar](#10-gambar)
11. [List (Daftar)](#11-list-daftar)
12. [Tabel](#12-tabel)
13. [Form](#13-form)
14. [Div dan Span](#14-div-dan-span)
15. [Atribut HTML](#15-atribut-html)
16. [Komentar di HTML](#16-komentar-di-html)
17. [Audio dan Video](#17-audio-dan-video)
18. [Sedikit Sentuhan CSS](#18-sedikit-sentuhan-css)
19. [Membuat Halaman Web Lengkap](#19-membuat-halaman-web-lengkap)
20. [Tips dan Langkah Selanjutnya](#20-tips-dan-langkah-selanjutnya)

---

## 1. Apa itu HTML?

HTML (HyperText Markup Language) adalah bahasa yang digunakan untuk membuat struktur halaman web. Bayangkan HTML seperti kerangka rumah — dia menentukan di mana pintu, jendela, dan ruangan berada, tapi belum dicat atau didekorasi.

Setiap halaman web yang kamu kunjungi (Google, Instagram, Wikipedia) dibangun menggunakan HTML sebagai dasarnya. HTML bekerja sama dengan dua teman lainnya:

- **HTML** → struktur/kerangka (apa yang ditampilkan)
- **CSS** → tampilan/desain (warna, layout, font)
- **JavaScript** → interaksi/perilaku (animasi, tombol yang berfungsi)

Di tutorial ini kita fokus dulu ke HTML.

### Bagaimana cara kerjanya?

HTML terdiri dari **tag-tag** yang memberi tahu browser "ini judul", "ini paragraf", "ini gambar", dan seterusnya. Browser (seperti Chrome atau Firefox) membaca tag-tag ini dan menampilkannya sebagai halaman web yang rapi.

---

## 2. Persiapan Alat

Untuk belajar HTML, kamu hanya butuh dua hal:

1. **Text editor** — aplikasi untuk menulis kode. Rekomendasi untuk pemula: [Visual Studio Code](https://code.visualstudio.com/) (gratis, populer, banyak tutorialnya).
2. **Browser** — Chrome, Firefox, Edge, atau apa saja yang sudah ada di komputermu.

Tidak perlu install software mahal atau ribet. Notepad bawaan Windows juga bisa dipakai, tapi VS Code akan membuat belajarmu lebih nyaman karena ada pewarnaan kode otomatis.

---

## 3. Membuat File HTML Pertama

Mari langsung praktik!

1. Buka VS Code (atau text editor pilihanmu).
2. Buat file baru, simpan dengan nama `index.html`. **Penting:** ekstensi file harus `.html`, bukan `.txt`.
3. Tulis kode berikut:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Halaman Pertamaku</title>
</head>
<body>
    <h1>Halo, Dunia!</h1>
    <p>Ini adalah halaman web pertama yang saya buat.</p>
</body>
</html>
```

4. Simpan file, lalu klik dua kali file tersebut di File Explorer — file akan terbuka di browser dan menampilkan tulisan "Halo, Dunia!" dengan paragraf di bawahnya.

Selamat, kamu baru saja membuat halaman web pertamamu!

---

## 4. Struktur Dasar HTML

Setiap file HTML memiliki struktur dasar yang sama. Mari kita bedah kode di atas baris per baris:

```html
<!DOCTYPE html>
```
Baris ini memberi tahu browser bahwa dokumen ini menggunakan HTML versi terbaru (HTML5). Selalu tulis ini di baris paling atas.

```html
<html>
...
</html>
```
Tag `<html>` adalah "pembungkus" seluruh isi halaman. Semua kode HTML lainnya harus berada di dalam tag ini.

```html
<head>
...
</head>
```
Bagian `<head>` berisi informasi tentang halaman yang **tidak ditampilkan langsung** ke pengunjung, seperti judul tab browser, deskripsi halaman, atau link ke file CSS.

```html
<body>
...
</body>
```
Bagian `<body>` berisi semua konten yang **akan ditampilkan** ke pengunjung — teks, gambar, tombol, dan sebagainya. Ini adalah bagian yang paling sering kamu sentuh.

### Analogi sederhana

Bayangkan `<html>` sebagai rumah, `<head>` sebagai dokumen administrasi rumah (sertifikat, alamat) yang tidak terlihat tamu, dan `<body>` sebagai ruangan-ruangan yang dilihat dan digunakan tamu.

---

## 5. Tag dan Elemen

**Tag** adalah kode yang diapit tanda kurung siku, contoh: `<p>`, `<h1>`, `<div>`.

Kebanyakan tag punya pasangan **pembuka** dan **penutup**:

```html
<p>Ini teks di dalam tag paragraf</p>
```

- `<p>` → tag pembuka
- `</p>` → tag penutup (perhatikan garis miring `/`)
- `Ini teks di dalam tag paragraf` → konten/isi

Gabungan dari tag pembuka + isi + tag penutup disebut **elemen**.

### Tag yang tidak butuh penutup

Beberapa tag berdiri sendiri tanpa konten dan tanpa tag penutup, contoh:

```html
<br>      <!-- membuat baris baru -->
<img>     <!-- menampilkan gambar -->
<hr>      <!-- membuat garis horizontal -->
```

Tag seperti ini disebut **self-closing** atau **void element**.

---

## 6. Heading (Judul)

HTML punya 6 level heading, dari `<h1>` (paling besar/penting) sampai `<h6>` (paling kecil).

```html
<h1>Ini Heading 1 - Paling Besar</h1>
<h2>Ini Heading 2</h2>
<h3>Ini Heading 3</h3>
<h4>Ini Heading 4</h4>
<h5>Ini Heading 5</h5>
<h6>Ini Heading 6 - Paling Kecil</h6>
```

**Tips:** Gunakan `<h1>` hanya satu kali per halaman untuk judul utama, lalu gunakan `<h2>`, `<h3>`, dst untuk sub-judul, seperti struktur daftar isi sebuah buku.

---

## 7. Paragraf dan Teks

Untuk menulis paragraf, gunakan tag `<p>`:

```html
<p>Ini adalah paragraf pertama. Kamu bisa menulis kalimat sepanjang yang kamu mau di sini.</p>
<p>Ini paragraf kedua, terpisah dari paragraf pertama.</p>
```

### Membuat baris baru tanpa paragraf baru

Gunakan `<br>` jika hanya ingin pindah baris tanpa membuat jarak antar-paragraf:

```html
<p>Alamat saya:<br>
Jl. Merdeka No. 10<br>
Yogyakarta</p>
```

### Garis pembatas

Gunakan `<hr>` untuk membuat garis horizontal pemisah konten:

```html
<p>Bagian pertama</p>
<hr>
<p>Bagian kedua</p>
```

---

## 8. Format Teks

HTML punya beberapa tag untuk mempercantik teks:

```html
<p><b>Teks tebal</b> atau <strong>teks penting (tebal)</strong></p>
<p><i>Teks miring</i> atau <em>teks dengan penekanan (miring)</em></p>
<p><u>Teks bergaris bawah</u></p>
<p><mark>Teks dengan highlight kuning</mark></p>
<p><small>Teks lebih kecil</small></p>
<p>Air<sub>2</sub>O (subscript) dan 10<sup>2</sup> (superscript)</p>
```

**Catatan tentang `<b>` vs `<strong>` dan `<i>` vs `<em>`:**
- `<b>` dan `<i>` hanya mengubah tampilan (bold/italic) tanpa makna khusus.
- `<strong>` dan `<em>` mengubah tampilan **dan** memberi tahu browser/pembaca layar bahwa teks ini penting/ditekankan. Untuk konten yang memang penting secara makna, lebih baik pakai `<strong>` dan `<em>`.

---

## 9. Link (Tautan)

Gunakan tag `<a>` (anchor) untuk membuat link, dengan atribut `href` untuk menentukan tujuan:

```html
<a href="https://www.google.com">Kunjungi Google</a>
```

### Membuka link di tab baru

```html
<a href="https://www.google.com" target="_blank">Buka Google di tab baru</a>
```

### Link ke halaman lain di folder yang sama

```html
<a href="tentang.html">Tentang Kami</a>
```

### Link ke bagian tertentu di halaman yang sama (anchor link)

```html
<a href="#bagian-kontak">Lompat ke bagian Kontak</a>

<!-- Di bagian bawah halaman -->
<h2 id="bagian-kontak">Kontak</h2>
```

### Link email

```html
<a href="mailto:contoh@email.com">Kirim Email</a>
```

---

## 10. Gambar

Gunakan tag `<img>` untuk menampilkan gambar. Tag ini wajib punya atribut `src` (sumber gambar) dan sebaiknya juga `alt` (teks alternatif):

```html
<img src="foto-kucing.jpg" alt="Foto kucing oren sedang tidur">
```

- `src` → lokasi file gambar (bisa nama file di folder yang sama, atau URL dari internet)
- `alt` → teks yang muncul jika gambar gagal dimuat, dan dibaca oleh pembaca layar untuk pengguna tunanetra

### Mengatur ukuran gambar

```html
<img src="foto-kucing.jpg" alt="Foto kucing" width="300" height="200">
```

### Menggunakan gambar dari internet

```html
<img src="https://contoh.com/gambar.jpg" alt="Deskripsi gambar">
```

### Menjadikan gambar sebagai link

```html
<a href="https://www.google.com">
    <img src="logo.png" alt="Logo Google">
</a>
```

---

## 11. List (Daftar)

Ada dua jenis daftar utama di HTML.

### Daftar tidak berurutan (bullet points)

```html
<ul>
    <li>Apel</li>
    <li>Jeruk</li>
    <li>Mangga</li>
</ul>
```

Hasilnya:
- Apel
- Jeruk
- Mangga

### Daftar berurutan (bernomor)

```html
<ol>
    <li>Bangun pagi</li>
    <li>Sarapan</li>
    <li>Berangkat sekolah</li>
</ol>
```

Hasilnya:
1. Bangun pagi
2. Sarapan
3. Berangkat sekolah

### Daftar bersarang (nested list)

```html
<ul>
    <li>Buah
        <ul>
            <li>Apel</li>
            <li>Jeruk</li>
        </ul>
    </li>
    <li>Sayur
        <ul>
            <li>Bayam</li>
            <li>Kangkung</li>
        </ul>
    </li>
</ul>
```

---

## 12. Tabel

Tabel dibuat dengan kombinasi beberapa tag:

```html
<table border="1">
    <tr>
        <th>Nama</th>
        <th>Umur</th>
        <th>Kota</th>
    </tr>
    <tr>
        <td>Budi</td>
        <td>25</td>
        <td>Yogyakarta</td>
    </tr>
    <tr>
        <td>Sari</td>
        <td>22</td>
        <td>Jakarta</td>
    </tr>
</table>
```

Penjelasan tag:
- `<table>` → pembungkus seluruh tabel
- `<tr>` → table row (baris)
- `<th>` → table header (judul kolom, otomatis tebal)
- `<td>` → table data (isi sel biasa)

**Catatan:** atribut `border="1"` hanya untuk latihan supaya garis tabel terlihat. Untuk tampilan yang lebih rapi nantinya kita pakai CSS.

---

## 13. Form

Form digunakan untuk menerima input dari pengguna, misalnya form login atau form pendaftaran.

```html
<form>
    <label for="nama">Nama:</label><br>
    <input type="text" id="nama" name="nama"><br><br>

    <label for="email">Email:</label><br>
    <input type="email" id="email" name="email"><br><br>

    <label for="password">Password:</label><br>
    <input type="password" id="password" name="password"><br><br>

    <label>Jenis Kelamin:</label><br>
    <input type="radio" id="pria" name="gender" value="pria">
    <label for="pria">Pria</label>
    <input type="radio" id="wanita" name="gender" value="wanita">
    <label for="wanita">Wanita</label><br><br>

    <input type="checkbox" id="setuju" name="setuju">
    <label for="setuju">Saya setuju dengan syarat dan ketentuan</label><br><br>

    <label for="negara">Pilih Negara:</label><br>
    <select id="negara" name="negara">
        <option value="id">Indonesia</option>
        <option value="my">Malaysia</option>
        <option value="sg">Singapura</option>
    </select><br><br>

    <label for="pesan">Pesan:</label><br>
    <textarea id="pesan" name="pesan" rows="4" cols="30"></textarea><br><br>

    <button type="submit">Kirim</button>
</form>
```

Penjelasan elemen penting:
- `<input type="text">` → kotak teks satu baris
- `<input type="email">` → kotak teks khusus email (browser akan validasi format)
- `<input type="password">` → kotak teks yang menyembunyikan karakter (titik-titik)
- `<input type="radio">` → pilihan tunggal (hanya bisa pilih satu)
- `<input type="checkbox">` → kotak centang (bisa pilih lebih dari satu)
- `<select>` dan `<option>` → dropdown/menu pilihan
- `<textarea>` → kotak teks panjang/multi-baris
- `<button>` → tombol
- `<label>` → label/keterangan untuk input (atribut `for` harus sama dengan `id` input agar saling terhubung)

---

## 14. Div dan Span

`<div>` dan `<span>` adalah tag "pembungkus" yang tidak memiliki tampilan khusus, tapi sangat berguna untuk mengelompokkan konten — biasanya supaya bisa diatur tampilannya dengan CSS nanti.

### `<div>` — pembungkus blok (mengambil satu baris penuh)

```html
<div>
    <h2>Judul Artikel</h2>
    <p>Ini adalah isi artikel yang dikelompokkan dalam satu div.</p>
</div>
```

### `<span>` — pembungkus dalam satu baris (inline)

```html
<p>Nama saya <span style="color: blue;">Budi</span> dan saya tinggal di Yogyakarta.</p>
```

Bedanya: `<div>` selalu membuat blok baru (seperti paragraf), sedangkan `<span>` hanya membungkus sebagian kecil teks di tengah kalimat tanpa memutus baris.

---

## 15. Atribut HTML

**Atribut** adalah informasi tambahan yang ditempelkan pada tag pembuka, untuk memberi instruksi lebih detail. Kita sudah memakai beberapa atribut di atas (`href`, `src`, `alt`, `type`, dll).

Format umum atribut:

```html
<tag atribut="nilai">Konten</tag>
```

Beberapa atribut yang sering dipakai di hampir semua tag:

```html
<p id="paragraf-utama">Paragraf dengan id unik</p>
<p class="teks-penting">Paragraf dengan class (bisa dipakai berulang)</p>
<p title="Ini adalah tooltip">Arahkan kursor ke sini untuk lihat tooltip</p>
<p style="color: red; font-size: 20px;">Paragraf dengan style langsung</p>
```

- `id` → pengenal unik, hanya boleh dipakai **satu kali** per halaman
- `class` → pengenal yang bisa dipakai **berkali-kali**, biasa dipakai untuk styling banyak elemen sekaligus
- `style` → menambahkan CSS langsung di tag (disebut inline style)
- `title` → menampilkan tooltip saat kursor diarahkan ke elemen

---

## 16. Komentar di HTML

Komentar adalah catatan dalam kode yang **tidak akan ditampilkan** di halaman web. Berguna untuk memberi catatan pengingat untuk dirimu sendiri atau orang lain yang membaca kodenya.

```html
<!-- Ini adalah komentar, tidak akan terlihat di browser -->
<p>Teks ini akan terlihat di browser.</p>

<!-- 
Komentar juga bisa
ditulis dalam beberapa baris
-->
```

---

## 17. Audio dan Video

### Menambahkan audio

```html
<audio controls>
    <source src="musik.mp3" type="audio/mpeg">
    Browser kamu tidak mendukung pemutar audio.
</audio>
```

### Menambahkan video

```html
<video width="320" height="240" controls>
    <source src="video.mp4" type="video/mp4">
    Browser kamu tidak mendukung pemutar video.
</video>
```

Atribut `controls` menampilkan tombol play/pause/volume bawaan browser.

---

## 18. Sedikit Sentuhan CSS

HTML mengatur struktur, tapi untuk mengatur **tampilan** (warna, ukuran, jarak), kita butuh CSS. Berikut cara paling dasar memasukkan CSS ke halaman HTML, supaya kamu punya bayangan awal sebelum mempelajarinya lebih dalam di tutorial lain.

### Cara 1: Inline style (langsung di tag)

```html
<p style="color: blue; font-size: 18px;">Paragraf berwarna biru</p>
```

### Cara 2: Internal style (di dalam `<head>`)

```html
<head>
    <style>
        p {
            color: green;
            font-family: Arial;
        }
        h1 {
            text-align: center;
        }
    </style>
</head>
```

### Cara 3: External style (file CSS terpisah, paling direkomendasikan)

File `style.css`:
```css
p {
    color: purple;
}
```

Di file HTML:
```html
<head>
    <link rel="stylesheet" href="style.css">
</head>
```

Cara ketiga ini yang paling baik dipakai untuk proyek nyata, karena memisahkan struktur (HTML) dan tampilan (CSS) sehingga lebih mudah dirawat.

---

## 19. Membuat Halaman Web Lengkap

Sekarang mari gabungkan semua yang sudah dipelajari menjadi satu halaman web sederhana, seperti halaman profil pribadi:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Profil Saya</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 40px;
            background-color: #f4f4f4;
        }
        h1 {
            color: #2c3e50;
        }
        .kontainer {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
        }
    </style>
</head>
<body>
    <div class="kontainer">
        <h1>Halo, Saya Budi!</h1>
        <img src="https://via.placeholder.com/150" alt="Foto profil Budi" width="150">

        <h2>Tentang Saya</h2>
        <p>Saya adalah seorang <strong>pemula</strong> yang baru belajar HTML. Saya tinggal di Yogyakarta dan sedang menikmati proses belajar membuat website.</p>

        <h2>Hobi Saya</h2>
        <ul>
            <li>Membaca buku</li>
            <li>Bermain gitar</li>
            <li>Jalan-jalan ke pantai</li>
        </ul>

        <h2>Kontak</h2>
        <table border="1">
            <tr>
                <th>Platform</th>
                <th>Username</th>
            </tr>
            <tr>
                <td>Email</td>
                <td>budi@email.com</td>
            </tr>
            <tr>
                <td>Instagram</td>
                <td>@budi_keren</td>
            </tr>
        </table>

        <h2>Hubungi Saya</h2>
        <form>
            <label for="pesan">Kirim Pesan:</label><br>
            <textarea id="pesan" name="pesan" rows="4" cols="40"></textarea><br><br>
            <button type="submit">Kirim</button>
        </form>

        <hr>
        <p><small>Terima kasih sudah berkunjung ke halaman saya!</small></p>
        <a href="#">Kembali ke Atas</a>
    </div>
</body>
</html>
```

Coba salin kode ini ke file `index.html` dan buka di browser. Kamu akan melihat halaman profil sederhana lengkap dengan foto, daftar hobi, tabel kontak, dan form pesan — semuanya hasil dari tag-tag yang sudah dipelajari di atas!

---

## 20. Tips dan Langkah Selanjutnya

### Tips belajar HTML

- **Praktik langsung**, jangan hanya membaca. Ketik ulang setiap contoh kode dengan tanganmu sendiri, jangan copy-paste, supaya lebih melekat di memori.
- **Eksperimen**, ubah-ubah nilai atau teks di contoh kode, lalu lihat apa yang berubah di browser.
- **Jangan takut error**. Halaman yang tidak tampil sesuai harapan adalah bagian normal dari proses belajar.
- Gunakan tombol klik kanan → **Inspect** di browser untuk melihat struktur HTML halaman web favoritmu dan belajar dari sana.

### Langkah selanjutnya setelah menguasai HTML

1. **CSS** — pelajari lebih dalam untuk mendesain tampilan (warna, layout, animasi sederhana).
2. **JavaScript** — pelajari untuk membuat halaman web yang interaktif (tombol berfungsi, validasi form, animasi).
3. **Responsive Design** — belajar membuat halaman yang tampil baik di HP maupun komputer.
4. **Git & GitHub** — belajar menyimpan dan membagikan kode proyekmu secara online.

Selamat belajar, dan semoga lancar perjalanan codingmu dari nol sampai bisa membuat website sendiri!

---

## 🤝 Kontribusi

Menemukan typo atau ingin menambahkan contoh? Silakan buat **pull request** atau buka **issue** di repository ini.

## 📄 Lisensi

Bebas digunakan, disalin, dan dimodifikasi untuk keperluan belajar maupun mengajar.

---

⭐ Jika tutorial ini membantu, jangan ragu untuk memberi **star** pada repository ini!
