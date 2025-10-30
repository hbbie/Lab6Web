# Lab6Web
Tugas Pertemua Pemrograman Web 7

Nama : Dhani Naufal Habibie

NIM : 312410300

KELAS : TI.24.A.4

# TUGAS & PERTANYAAN

1. Refactor Layout Praktikum 4
Ambil layout web sederhana dari Praktikum 4. Buat ulang layout tersebut menggunakan

Bootstrap Grid System.

○ Gunakan <nav> Bootstrap untuk bagian navigasi

○ Gunakan class .row dan .col-md-8 untuk main content dan .col-md-4 untuk sidebar

○ Gunakan komponen .card Bootstrap untuk menggantikan .widget-box

○ Gunakan komponen .card untuk menggantikan .box (bagian "Heading" yang berisi 3
kolom)

○ Anda tidak diperbolehkan menggunakan CSS float atau clear manual.

Kode Program :

``` html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Travel Blog Bootstrap</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <!-- NAVBAR -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
    <div class="container">
      <a class="navbar-brand fw-bold" href="#">TravelKu</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div id="navbarNav" class="collapse navbar-collapse">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link active" href="#">Beranda</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Destinasi</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Tips</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Kontak</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- MAIN CONTENT + SIDEBAR -->
  <div class="container my-4">
    <div class="row">
      <!-- MAIN CONTENT -->
      <div class="col-md-8">
        <div class="card mb-4 shadow-sm">
          <img src="https://source.unsplash.com/800x400/?beach" class="card-img-top" alt="Pantai">
          <div class="card-body">
            <h3 class="card-title">Petualangan Seru di Pulau Lombok</h3>
            <p class="card-text">Lombok adalah salah satu destinasi wisata paling indah di Indonesia. Dari pantai berpasir putih hingga Gunung Rinjani yang megah, semua bisa kamu jelajahi di sini.</p>
            <a href="#" class="btn btn-primary">Baca Selengkapnya</a>
          </div>
        </div>
      </div>

      <!-- SIDEBAR -->
      <div class="col-md-4">
        <div class="card mb-4">
          <div class="card-header bg-primary text-white">Tentang Penulis</div>
          <div class="card-body">
            <p>Hai! Saya Rina, seorang travel blogger yang suka menjelajahi tempat-tempat baru di Indonesia. Yuk, ikuti petualangan saya!</p>
          </div>
        </div>
      </div>
    </div>

    <!-- TIGA KOTAK (DESTINASI POPULER) -->
    <div class="row mt-4">
      <div class="col-md-4">
        <div class="card text-center shadow-sm">
          <img src="https://source.unsplash.com/300x200/?mountain" class="card-img-top" alt="Gunung">
          <div class="card-body">
            <h5 class="card-title">Gunung Bromo</h5>
            <p class="card-text">Panorama matahari terbit yang menakjubkan.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4">
        <div class="card text-center shadow-sm">
          <img src="https://source.unsplash.com/300x200/?temple" class="card-img-top" alt="Candi">
          <div class="card-body">
            <h5 class="card-title">Candi Borobudur</h5>
            <p class="card-text">Warisan budaya dunia yang menawan.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4">
        <div class="card text-center shadow-sm">
          <img src="https://source.unsplash.com/300x200/?island" class="card-img-top" alt="Pulau">
          <div class="card-body">
            <h5 class="card-title">Pulau Komodo</h5>
            <p class="card-text">Petualangan seru bersama naga raksasa!</p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- FOOTER -->
  <footer class="bg-dark text-white text-center py-3 mt-4">
    <p class="mb-0">&copy; 2025 TravelKu | Jelajahi Dunia Tanpa Batas</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```
Outputnya :
<img width="1902" height="919" alt="image" src="https://github.com/user-attachments/assets/8d5f8aa4-f6be-4091-b516-4a182722b427" />

2. Refactor Form Praktikum 5

Ambil salah satu form dari Praktikum 5 (misalnya Form Input 23atau Form Button 24).

Buat ulang form tersebut agar terlihat rapi menggunakan class-class form Bootstrap (.form-

control, .form-label, .btn).

Kode Program :

``` html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Formulir Pendaftaran Kursus (Bootstrap)</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light">

  <div class="container py-5">
    <div class="row justify-content-center">
      <div class="col-md-6">
        <div class="card shadow-lg border-0">
          <div class="card-header bg-success text-white text-center">
            <h4>Formulir Pendaftaran Kursus</h4>
          </div>
          <div class="card-body">
            <form>
              <div class="mb-3">
                <label for="nama" class="form-label">Nama Lengkap</label>
                <input type="text" id="nama" class="form-control" placeholder="Masukkan nama Anda">
              </div>

              <div class="mb-3">
                <label for="email" class="form-label">Alamat Email</label>
                <input type="email" id="email" class="form-control" placeholder="nama@email.com">
              </div>

              <div class="mb-3">
                <label for="telepon" class="form-label">Nomor Telepon</label>
                <input type="tel" id="telepon" class="form-control" placeholder="08xxxxxxxxxx">
              </div>

              <div class="mb-3">
                <label for="kursus" class="form-label">Pilih Kursus</label>
                <select id="kursus" class="form-select">
                  <option selected disabled>-- Pilih Kursus --</option>
                  <option>Desain Grafis</option>
                  <option>Web Development</option>
                  <option>Bahasa Inggris</option>
                  <option>Digital Marketing</option>
                </select>
              </div>

              <div class="mb-3">
                <label for="pesan" class="form-label">Catatan Tambahan</label>
                <textarea id="pesan" class="form-control" rows="3" placeholder="Tuliskan hal yang perlu kami ketahui"></textarea>
              </div>

              <button type="submit" class="btn btn-success w-100">Daftar Sekarang</button>
            </form>
          </div>
          <div class="card-footer text-center text-muted">
            <small>© 2025 KursusOnline.id</small>
          </div>
        </div>
      </div>
    </div>
  </div>

</body>
</html>

```
Hasil Outputnya :

<img width="745" height="610" alt="image" src="https://github.com/user-attachments/assets/4b28bda2-f6bf-4f3d-88d0-50648bb4634e" />

3. Tugas: Buat Halaman Portfolio Sederhana

Buat satu halaman HTML baru (portfolio.html) menggunakan Bootstrap yang berisi:

a. Sebuah Navbar di bagian atas.

b. Sebuah section "Tentang Saya" di dalam .container dengan 1 baris (.row) dan 2 kolom
(.col):

* Kolom kiri (.col-md-4) berisi foto Anda (gunakan <img> dengan class .img-fluid).

* Kolom kanan (.col-md-8) berisi nama dan deskripsi diri Anda.

c. Sebuah section "Portfolio Saya" di dalam .container dengan 1 baris (.row) dan 3 kolom
(.col-md-4):

* Setiap kolom berisi satu komponen .card yang merepresentasikan satu proyek (beri
gambar dummy dan deskripsi singkat).

Kode Program :
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Portfolio Habibie Beckham</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

  <style>
    /* Mengecilkan ukuran foto profil */
    .foto-profil {
      width: 220px;   /* ubah sesuai kebutuhan (default: 220px) */
      height: 280px;
      object-fit: cover;
      border-radius: 50%;
      border: 4px solid #fff;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container">
      <a class="navbar-brand fw-bold" href="#">Habibie Portfolio</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navMenu">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div id="navMenu" class="collapse navbar-collapse">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#tentang">Tentang</a></li>
          <li class="nav-item"><a class="nav-link" href="#karya">Karya</a></li>
          <li class="nav-item"><a class="nav-link" href="#kontak">Kontak</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Tentang Saya -->
  <section id="tentang" class="container my-5">
    <div class="row align-items-center">
      <div class="col-md-4 text-center">
        <img src="foto 1.jpg" class="foto-profil" alt="Foto Habibie">
      </div>
      <div class="col-md-8">
        <h2 class="fw-bold">Habibie Beckham</h2>
        <p>Hai! Aku Habibie, mahasiswa jurusan Informatika yang suka mendesain website dan aplikasi dengan tampilan menarik. Fokusku ada di front-end development dan UI/UX design. Aku juga senang berkolaborasi dalam proyek kreatif!</p>
      </div>
    </div>
  </section>

  <!-- Karya -->
  <section id="karya" class="container my-5">
    <h3 class="text-center mb-4 fw-bold">Karya Terbaru</h3>
    <div class="row g-4">
      <div class="col-md-4">
        <div class="card h-100 shadow-sm">
          <div class="card-body">
            <h5 class="card-title">Karya 1</h5>
            <p class="card-text">Desain website portfolio interaktif menggunakan HTML, CSS, dan Bootstrap.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4">
        <div class="card h-100 shadow-sm">
          <div class="card-body">
            <h5 class="card-title">Karya 2</h5>
            <p class="card-text">Aplikasi “To-Do List” berbasis JavaScript dengan tampilan yang minimalis.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4">
        <div class="card h-100 shadow-sm">
          <div class="card-body">
            <h5 class="card-title">Karya 3</h5>
            <p class="card-text">Landing page produk kecantikan yang responsif dan modern.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Kontak -->
  <section id="kontak" class="container my-5">
    <h3 class="text-center mb-4 fw-bold">Hubungi Saya</h3>
    <div class="row justify-content-center">
      <div class="col-md-6">
        <div class="card shadow">
          <div class="card-body">
            <form>
              <div class="mb-3">
                <label for="nama" class="form-label">Nama</label>
                <input type="text" id="nama" class="form-control" placeholder="Masukkan nama Anda">
              </div>
              <div class="mb-3">
                <label for="email" class="form-label">Email</label>
                <input type="email" id="email" class="form-control" placeholder="nama@email.com">
              </div>
              <div class="mb-3">
                <label for="pesan" class="form-label">Pesan</label>
                <textarea id="pesan" class="form-control" rows="3" placeholder="Tuliskan pesan Anda"></textarea>
              </div>
              <button type="submit" class="btn btn-dark w-100">Kirim Pesan</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-dark text-white text-center py-3 mt-5">
    <p class="mb-0">&copy; 2025 Habibie Beckham | Dibuat dengan ❤️ dan Bootstrap</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```
Hasilnya :
<img width="1870" height="926" alt="image" src="https://github.com/user-attachments/assets/af257070-d63f-4e2d-8c6e-28c9ca71f6b9" />
