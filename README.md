<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Portofolio — Nama Anda</title>
  <meta name="description" content="Portofolio sederhana: about, projects, contact" />
  <style>
    :root{--bg:#0f1724;--card:#0b1220;--muted:#98a0b3;--accent:#6ee7b7;--white:#eef2f6}
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;color:var(--white);background:linear-gradient(180deg,#071126 0%, #071a2a 100%);}
    .container{max-width:1000px;margin:32px auto;padding:24px}
    header{display:flex;align-items:center;justify-content:space-between;margin-bottom:28px}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:48px;height:48px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#60a5fa);display:flex;align-items:center;justify-content:center;color:#05201a;font-weight:700}
    nav a{color:var(--muted);text-decoration:none;margin-left:18px;font-weight:600}
    nav a:hover{color:var(--white)}

    .hero{display:grid;grid-template-columns:1fr 380px;gap:28px;align-items:center;margin-bottom:28px}
    .intro h1{font-size:28px;margin:0 0 8px}
    .intro p{color:var(--muted);margin:0 0 16px;line-height:1.5}
    .cta{display:flex;gap:10px}
    .btn{padding:10px 14px;border-radius:8px;border:0;cursor:pointer;font-weight:700}
    .btn-primary{background:var(--accent);color:#05201a}
    .btn-ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--white)}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:12px;padding:18px}
    .profile{display:flex;gap:14px;align-items:center}
    .avatar{width:72px;height:72px;border-radius:12px;background:linear-gradient(135deg,#3b82f6,#06b6d4);display:flex;align-items:center;justify-content:center;font-weight:800}
    .meta small{color:var(--muted)}

    .projects{margin-top:18px;display:grid;grid-template-columns:repeat(2,1fr);gap:16px}
    .project{padding:14px;border-radius:10px;background:rgba(255,255,255,0.02)}
    .project h3{margin:0 0 8px;font-size:16px}
    .project p{margin:0;color:var(--muted);font-size:14px}

    footer{margin-top:28px;color:var(--muted);font-size:14px;text-align:center}

    /* responsive */
    @media (max-width:900px){
      .hero{grid-template-columns:1fr;}
      .projects{grid-template-columns:1fr}
      nav a{margin-left:12px}
    }

    /* small utilities */
    .muted{color:var(--muted)}
    .tag{display:inline-block;padding:6px 8px;border-radius:999px;background:rgba(255,255,255,0.02);font-size:12px;margin-right:6px}
    .contact-form{display:flex;flex-direction:column;gap:8px}
    input,textarea{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:10px;border-radius:8px;color:var(--white);resize:vertical}
    input::placeholder,textarea::placeholder{color:rgba(255,255,255,0.35)}
    .small{font-size:13px;color:var(--muted)}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">NA</div>
        <div>
          <div style="font-weight:800">Nama Anda</div>
          <div class="small">Frontend Developer • Designer</div>
        </div>
      </div>
      <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div class="intro card">
          <h1>Halo — saya Nama Anda</h1>
          <p>Saya pembuat antarmuka yang menyenangkan, membuat website yang sederhana, cepat, dan mudah digunakan. Saya suka membangun proyek yang memecahkan masalah nyata.</p>
          <div class="cta">
            <button class="btn btn-primary" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">Hubungi saya</button>
            <a class="btn btn-ghost" href="#projects">Lihat proyek</a>
          </div>
          <div style="margin-top:16px">
            <span class="tag">HTML</span><span class="tag">CSS</span><span class="tag">JavaScript</span>
          </div>
        </div>

        <aside class="card">
          <div class="profile">
            <div class="avatar">ND</div>
            <div class="meta">
              <div style="font-weight:700">Nama Anda</div>
              <small class="muted">Jakarta, Indonesia • open to work</small>
            </div>
          </div>

          <div class="projects" style="margin-top:16px">
            <div class="project">
              <h3>Project A</h3>
              <p class="muted">Situs toko online sederhana — HTML/CSS/JS</p>
            </div>
            <div class="project">
              <h3>Project B</h3>
              <p class="muted">Dashboard analitik — chart & interaksi</p>
            </div>
          </div>
        </aside>
      </section>

      <section id="about" class="card" style="margin-bottom:18px">
        <h2 style="margin-top:0">Tentang saya</h2>
        <p class="muted">Saya memiliki pengalaman membangun antarmuka web yang responsif. Fokus saya pada aksesibilitas, performa, dan desain yang bersih.</p>
        <ul class="small muted">
          <li>Pengalaman: 2+ tahun</li>
          <li>Keahlian: HTML, CSS, JavaScript, Git</li>
          <li>Bahasa: Indonesia, Inggris dasar</li>
        </ul>
      </section>

      <section id="projects">
        <h2 style="margin-bottom:12px">Proyek</h2>
        <div class="projects">
          <div class="project card">
            <h3>Website Profil Sekolah</h3>
            <p class="muted">Membangun website profil sekolah dengan halaman informasi guru, galeri, dan kontak.</p>
            <div style="margin-top:8px"><a href="#" class="small muted">Lihat demo</a></div>
          </div>

          <div class="project card">
            <h3>Aplikasi To‑Do Sederhana</h3>
            <p class="muted">Aplikasi manajemen tugas dengan localStorage dan filter.</p>
            <div style="margin-top:8px"><a href="#" class="small muted">Lihat kode</a></div>
          </div>

          <div class="project card">
            <h3>Landing Page Produk</h3>
            <p class="muted">Landing page responsif untuk produk digital dengan CTA yang jelas.</p>
            <div style="margin-top:8px"><a href="#" class="small muted">Lihat demo</a></div>
          </div>

          <div class="project card">
            <h3>Portfolio Interaktif</h3>
            <p class="muted">Portofolio interaktif dengan animasi ringan dan navigasi yang mudah.</p>
            <div style="margin-top:8px"><a href="#" class="small muted">Lihat</a></div>
          </div>
        </div>
      </section>

      <section id="contact" class="card" style="margin-top:18px">
        <h2 style="margin-top:0">Kontak</h2>
        <p class="muted">Ingin bekerja sama atau tanya‑tanya? Kirim pesan lewat form ini (form tidak terkirim karena tidak ada backend — instruksi di bawah).</p>
        <form class="contact-form" onsubmit="handleSubmit(event)">
          <input id="name" placeholder="Nama lengkap" required />
          <input id="email" type="email" placeholder="Email" required />
          <textarea id="message" rows="5" placeholder="Pesan" required></textarea>
          <div style="display:flex;gap:8px;align-items:center">
            <button class="btn btn-primary" type="submit">Kirim</button>
            <div class="small muted">atau hubungi: <strong>email@contoh.com</strong></div>
          </div>
        </form>
      </section>

    </main>

    <footer>
      &copy; <span id="year"></span> Nama Anda — Dibuat dengan sederhana.
    </footer>
  </div>

  <script>
    // small scripts: year, form handler
    document.getElementById('year').textContent = new Date().getFullYear();

    function handleSubmit(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const message = document.getElementById('message').value.trim();
      if(!name || !email || !message){
        alert('Mohon lengkapi semua field.');
        return;
      }
      // Tidak ada backend di contoh ini. Anda bisa sambungkan ke email/endpoint.
      alert('Terima kasih, pesan Anda berhasil diproses (contoh).');
      e.target.reset();
    }
  </script>
</body>
</html>
