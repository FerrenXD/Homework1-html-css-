<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mengenal Devops</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body { font-family: 'Segoe UI', sans-serif; line-height: 1.6; background: #fdfdfd; color: #333; }
    a { text-decoration: none; color: inherit; }
    img { max-width: 100%; display: block; }
    .container { width: 90%; max-width: 1200px; margin: auto; }

    header { background: #fff; padding: 20px 0; border-bottom: 1px solid #eee; position: sticky; top: 0; z-index: 1000; }
    .navbar { display: flex; justify-content: space-between; align-items: center; }
    .navbar h1 { font-size: 24px; color: #0077ff; font-weight: bold; }
    .nav-links { display: flex; gap: 20px; }
    .nav-links a { font-weight: 600; color: #444; transition: color 0.3s; }
    .nav-links a:hover { color: #0077ff; }

    .hero { background: #0077ff; color: white; padding: 100px 20px; text-align: center; }
    .hero h2 { font-size: 48px; margin-bottom: 20px; }
    .hero p { font-size: 20px; margin-bottom: 30px; }

    /* tombol continue ungu */
    .btn-primary {
      background: #800080; color: #fff;
      padding: 12px 30px; border-radius: 5px;
      font-weight: bold; transition: background 0.3s, transform 0.1s ease-in-out;
      display: inline-block; cursor: pointer; user-select: none;
    }
    .btn-primary:hover { background: #a020f0; }
    .btn-primary:active { transform: scale(1.1); }

    section { padding: 80px 0; }
    .section-title { text-align: center; margin-bottom: 40px; }
    .section-title h3 { font-size: 32px; margin-bottom: 10px; color: #0077ff; font-weight: 700; }
    .section-title p { color: #333; font-size: 18px; line-height: 1.6; font-weight: 400; }

    .about p { max-width: 700px; margin: 0 auto; text-align: center; font-size: 18px; color: #333; line-height: 1.6; font-weight: 400; }

    /* kotak ungu terang */
    .services-grid { display: flex; flex-direction: column; gap: 30px; }
    .service { background: #a64ca6; color: #fff; padding: 30px; border-radius: 8px; text-align: center; box-shadow: 0 4px 10px rgba(0,0,0,0.15); }
    .service h4 { font-size: 20px; margin-bottom: 10px; color: #ffd700; }
    .service p { color: #f5f5f5; font-size: 18px; line-height: 1.6; font-weight: 400; }

    @media (min-width: 768px) {
      .services-grid { flex-direction: row; justify-content: space-between; }
      .service { flex: 1; }
    }

    /* Contact */
    .contact-links {
      display: flex; flex-wrap: wrap; gap: 20px; justify-content: center;
    }
    .contact-links a {
      background: #a64ca6; color: white; padding: 12px 25px; border-radius: 6px;
      font-weight: bold; width: 180px; text-align: center; transition: background 0.3s;
    }
    .contact-links a:hover { background: #c46cc4; }

    /* Back to Top */
    .back-to-top {
      position: fixed; bottom: 20px; right: 20px;
      background: #a64ca6; color: #fff; padding: 12px 20px;
      border-radius: 6px; font-weight: bold;
      transition: background 0.3s, transform 0.2s;
      z-index: 1000;
    }
    .back-to-top:hover { background: #c46cc4; transform: scale(1.1); }

    footer { background: #222; color: #bbb; text-align: center; padding: 30px 0; margin-top: 40px; }
    .footer-links { margin-top: 10px; }
    .footer-links a { color: #bbb; margin: 0 10px; font-size: 14px; }
  </style>
</head>
<body>

  <header>
    <div class="container navbar">
      <h1>Materi</h1>
      <nav>
        <div class="nav-links">
          <a href="#home">Home</a>
          <a href="#Pengertian">Pengertian</a>
          <a href="#KarirDevops">Karir</a>
          <a href="#Fungsi">Fungsi</a>
          <a href="#Tujuan">Tujuan</a>
          <a href="#Kesimpulan">Kesimpulan</a>
          <a href="#contact">Contact</a>
        </div>
      </nav>
    </div>
  </header>

  <!-- Hero -->
  <section class="hero" id="home">
    <div class="container">
      <h2>Mengenal Development And Operation (DEVOPS)</h2>
      <p>Materi Tentang Devops.Materi Dapet Dari Hasil Saya Belajar Sedikit Dan Dibantu Beberapa Web,selamat belajar :P</p>
      <a href="#Pengertian" class="btn-primary">Get Started :)</a>
    </div>
  </section>

  <!-- Pengertian -->
  <section class="Pengertian" id="Pengertian">
    <div class="container">
      <div class="section-title">
        <h3>Pengertian</h3>
        <p>DevOps adalah sebuah pendekatan modern dalam pengembangan perangkat lunak yang menyatukan <b>Development</b> (Dev) dan <b>Operations</b> (Ops). 
        Tujuannya adalah mempercepat proses pembuatan aplikasi, meningkatkan kualitas, sekaligus menjaga stabilitas sistem.</p>
      </div>
      <p><b>Development (Dev):</b> bertugas merancang dan membangun aplikasi, menambahkan fitur, menulis kode, serta melakukan pengujian.</p>
      <p><b>Operations (Ops):</b> fokus pada pengelolaan infrastruktur, deployment, monitoring, serta memastikan aplikasi berjalan aman dan stabil di produksi.</p>
      <p style="text-align:center; max-width:700px; margin:30px auto; font-style:italic; color:#444;">
        Singkatnya, DevOps bukan hanya soal teknologi, tapi juga budaya kerja kolaboratif yang membuat tim lebih cepat, lebih gesit, dan lebih solid.
      </p>
      <div style="text-align:center; margin-top:30px;">
        <a href="#KarirDevops" class="btn-primary">Continue</a>
      </div>
    </div>
  </section>

  <!-- Karir DevOps -->
  <section id="KarirDevops">
    <div class="container">
      <div class="section-title">
        <h3>Karir DevOps</h3>
        <p>Jenjang karir DevOps Engineer terbuka dari level pemula hingga manajerial. Berikut beberapa tahapannya:</p>
      </div>
      <div class="services-grid">
        <div class="service">
          <h4>Junior DevOps Engineer</h4>
          <p>Cocok untuk pengalaman kerja kurang dari 1–3 tahun. Pada tahap ini fokus belajar sambil praktek bersama tim yang lebih senior.</p>
        </div>
        <div class="service">
          <h4>Senior DevOps Engineer</h4>
          <p>Dengan pengalaman 3–5 tahun lebih, biasanya sudah menguasai coding, automation, dan software delivery yang kompleks.</p>
        </div>
        <div class="service">
          <h4>Manajer DevOps</h4>
          <p>Posisi leadership yang memimpin tim DevOps, mengatur strategi deployment, serta memastikan kolaborasi antar divisi berjalan lancar.</p>
        </div>
      </div>
      <div style="text-align:center; margin-top:30px;">
        <a href="#Fungsi" class="btn-primary">Continue</a>
      </div>
    </div>
  </section>

  <!-- Fungsi -->
  <section id="Fungsi">
    <div class="container">
      <div class="section-title">
        <h3>Fungsi</h3>
        <p>Beberapa fungsi penting penerapan DevOps dalam perusahaan:</p>
      </div>
      <div class="services-grid">
        <div class="service">
          <h4>Kolaborasi Tim</h4>
          <p>Menyatukan tim developer dan operasi agar komunikasi lebih lancar dan produktif.</p>
        </div>
        <div class="service">
          <h4>Otomatisasi Proses</h4>
          <p>Menggunakan tools CI/CD untuk otomatisasi build, test, dan deployment.</p>
        </div>
        <div class="service">
          <h4>Monitoring & Feedback</h4>
          <p>Melakukan monitoring aplikasi real-time serta mendapatkan feedback cepat dari pengguna.</p>
        </div>
      </div>
      <div style="text-align:center; margin-top:30px;">
        <a href="#Tujuan" class="btn-primary">Continue</a>
      </div>
    </div>
  </section>

  <!-- Tujuan -->
  <section id="Tujuan">
    <div class="container">
      <div class="section-title">
        <h3>Tujuan</h3>
        <p>Tujuan utama penerapan DevOps bagi perusahaan:</p>
      </div>
      <div class="services-grid">
        <div class="service">
          <h4>Menghemat Waktu</h4>
          <p>Mempercepat eksekusi produk digital, mulai dari perencanaan hingga delivery.</p>
        </div>
        <div class="service">
          <h4>Cepat Beradaptasi</h4>
          <p>Kolaborasi tim memudahkan perusahaan berinovasi menghadapi persaingan.</p>
        </div>
        <div class="service">
          <h4>Pergerakan Bisnis Cepat</h4>
          <p>Kendala dalam pengembangan bisa teratasi lebih cepat sehingga bisnis lebih gesit.</p>
        </div>
        <div class="service">
          <h4>Menjaga Stabilitas & Kualitas</h4>
          <p>Penerapan CI/CD menghasilkan produk yang andal, stabil, dan minim bug.</p>
        </div>
      </div>
      <div style="text-align:center; margin-top:30px;">
        <a href="#Kesimpulan" class="btn-primary">Continue</a>
      </div>
    </div>
  </section>

  <!-- Kesimpulan -->
  <section id="Kesimpulan">
    <div class="container">
      <div class="section-title">
        <h3>Kesimpulan</h3>
        <p>evOps adalah instrumen lingkungan kerja pada perusahaan IT yang sedang berkembang saat ini. Prinsip ini dibuat dan digunakan untuk mengatasi berbagai permasalahan yang ada perusahaan IT untuk mengatur alur source code dalam hal pengembangan dan operasional.

“Kepemimpinan yang efektif adalah mengutamakan hal terpenting. Manajemen yang efektif adalah disiplin dan just do it.” (Stephen Covey)

Saat ini, DevOps Engineer menjadi salah satu profesi yang sedang berkembang dan prospek di masa mendatang. Kamu hanya cukup memenuhi persyaratan dan skill yang dibutuhkan perusahaan melalui rekrutmen kerja.</p>
      </div>
      <div style="text-align:center; margin-top:30px;">
        <a href="#contact" class="btn-primary">Continue</a>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <div class="container">
      <div class="section-title">
        <h3>Contact</h3>
        <p>Hubungi saya melalui platform berikut:</p>
      </div>
   <div class="contact-links">
  <a href="https://wa.me/+6282118317394" target="_blank">WhatsApp</a>
  <a href="https://github.com/FerrenXD" target="_blank">GitHub</a>
  <a href="https://instagram.com/LionelFerren" target="_blank">Instagram</a>
  <a href="https://youtube.com/@LionelFerrenXD" target="_blank">YouTube</a>
  <a href=""
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container">
      <p>&copy; XD </p>
      <div class="footer-links">
        <a href="#">Ubah Sedikit Saja :P</a> | <a href="#">Idea And Code By Ferren</a>
      </div>
    </div>
  </footer>

  <!-- Back to Top -->
  <a href="#home" class="back-to-top">Back to Top</a>

</body>
</html>
