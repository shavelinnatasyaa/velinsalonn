<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Velin Beauty Care & Spa — Daftar Harga & Layanan</title>

  <!-- Fonts: elegant headings + clean body -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@500;600;700&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">

  <meta name="description" content="Velin Beauty Care & Spa — Layanan profesional: Potong, Smoothing, Warna, Creambath, Hair Care, Blow Perm. Kontak & peta tersedia.">

  <style>
    :root{
      --white:#ffffff;
      --bg:#fbf6fc;
      --accent:#9b59b6;      /* primary purple */
      --accent-2:#7b1fa2;    /* deeper purple */
      --muted:#6b6b6b;
      --card:#ffffff;
      --radius:14px;
      --shadow: 0 18px 45px rgba(123,31,162,0.09);
      --wa: "https://wa.me/6285785716869";
    }

    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:'Poppins',system-ui,-apple-system,Segoe UI,Roboto,'Helvetica Neue',Arial;background:linear-gradient(180deg,var(--bg),#fff);color:#222;-webkit-font-smoothing:antialiased}
    a{color:inherit;text-decoration:none}

    /* page container */
    .wrap{max-width:1200px;margin:0 auto;padding:28px 20px}

    /* header */
    header{display:flex;align-items:center;justify-content:space-between;gap:18px;padding:10px 0}
    .brand{display:flex;align-items:center;gap:14px}
    .logo{width:64px;height:64px;border-radius:12px;background:linear-gradient(135deg,#fff,#f6eff8);display:grid;place-items:center;font-family:'Cormorant Garamond',serif;color:var(--accent-2);font-weight:700;font-size:22px;box-shadow:0 8px 28px rgba(123,31,162,0.12)}
    .brand h1{font-family:'Cormorant Garamond',serif;margin:0;font-size:1.25rem;color:var(--accent-2)}
    nav{display:flex;gap:10px;align-items:center}
    nav a{color:var(--muted);font-weight:600;padding:8px 10px;border-radius:8px}
    nav a:hover{background:rgba(155,89,182,0.06);color:var(--accent-2)}
    .btn-book{background:linear-gradient(90deg,var(--accent),var(--accent-2));color:#fff;padding:10px 14px;border-radius:999px;font-weight:700;box-shadow:0 10px 26px rgba(123,31,162,0.12)}

    /* hero */
    .hero{
      margin-top:6px;border-radius:18px;overflow:hidden;position:relative;display:flex;align-items:center;justify-content:center;
      min-height:56vh;
      background:
        linear-gradient(180deg, rgba(123,31,162,0.28), rgba(123,31,162,0.16)),
        url('https://images.unsplash.com/photo-1524758631624-e2822e304c36?auto=format&fit=crop&w=1600&q=80') center/cover no-repeat;
      box-shadow:var(--shadow);
    }
    .hero-inner{padding:56px 22px;text-align:center;color:#fff;max-width:980px}
    .hero h2{font-family:'Cormorant Garamond',serif;font-size:2.6rem;margin:0 0 8px;line-height:1}
    .hero p{margin:0 auto 18px;max-width:820px;opacity:0.98;font-size:1.03rem}
    .cta-row{display:flex;gap:12px;justify-content:center;flex-wrap:wrap}
    .cta-ghost{background:rgba(255,255,255,0.95);color:var(--accent-2);padding:12px 18px;border-radius:999px;font-weight:700;box-shadow:0 8px 20px rgba(0,0,0,0.06)}
    .cta-primary{background:linear-gradient(90deg,var(--accent),var(--accent-2));color:#fff;padding:12px 18px;border-radius:999px;font-weight:800;box-shadow:0 12px 30px rgba(123,31,162,0.14)}

    /* section headings */
    .section{padding:56px 0}
    .section .title{font-family:'Cormorant Garamond',serif;color:var(--accent-2);font-size:1.6rem;margin:0;text-align:center}
    .section .subtitle{color:var(--muted);text-align:center;margin-top:8px;max-width:860px;margin-left:auto;margin-right:auto}

    /* price list grid (per category card) */
    .category-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:22px;margin-top:22px}
    .category-card{background:var(--card);border-radius:12px;overflow:hidden;box-shadow:var(--shadow);border:1px solid rgba(123,31,162,0.06);display:flex;flex-direction:column;transition:transform .25s ease}
    .category-card:hover{transform:translateY(-8px)}
    .card-media{height:220px;background-size:cover;background-position:center}
    .card-body{padding:18px;display:flex;flex-direction:column;gap:10px}
    .cat-title{font-family:'Cormorant Garamond',serif;color:var(--accent-2);font-size:1.05rem;margin:0}
    .cat-desc{color:var(--muted);font-size:.95rem;margin:0}

    .price-list{margin-top:8px}
    .price-row{display:flex;justify-content:space-between;align-items:flex-start;padding:10px 0;border-bottom:1px dashed rgba(0,0,0,0.04)}
    .price-row:last-child{border-bottom:0}
    .price-left{font-weight:600;color:#222}
    .price-right{color:var(--muted)}
    .price-note{color:var(--muted);font-size:.92rem;margin-top:8px}

    .card-footer{display:flex;gap:12px;align-items:center;margin-top:12px;flex-wrap:wrap}
    .btn-wa{background:linear-gradient(90deg,var(--accent),var(--accent-2));color:#fff;padding:10px 12px;border-radius:10px;font-weight:800;box-shadow:0 10px 26px rgba(123,31,162,0.12)}

    /* If lots of lines: two-column list inside card */
    .price-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:8px}

    /* socials (large cards above map) */
    .socials-large{display:flex;gap:14px;align-items:stretch;margin-top:18px;flex-wrap:wrap}
    .social-card{flex:1;min-width:220px;background:linear-gradient(180deg,#fff,#fbf8ff);border-radius:12px;padding:18px;display:flex;align-items:center;gap:12px;border:1px solid rgba(123,31,162,0.06);box-shadow:0 14px 36px rgba(123,31,162,0.06)}
    .social-card img{width:48px;height:48px;flex-shrink:0;border-radius:8px}
    .social-card .info{display:flex;flex-direction:column}
    .social-card .label{font-weight:700;color:var(--accent-2)}
    .social-card .meta{color:var(--muted);font-size:.95rem}
    .social-card .action{margin-top:8px;font-weight:800;color:#fff;background:var(--accent-2);padding:8px 10px;border-radius:8px;display:inline-block}

    /* testimonials & gallery */
    .testi-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:18px}
    .testi-card{background:linear-gradient(180deg,#fff,#fbf8ff);padding:18px;border-radius:12px;box-shadow:0 10px 30px rgba(123,31,162,0.06);border:1px solid rgba(123,31,162,0.06)}
    .testi-card p{font-style:italic;margin:0;color:#333}
    .testi-author{margin-top:10px;font-weight:700;color:var(--accent-2)}

    .gallery-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:12px;margin-top:18px}
    .gallery-grid img{width:100%;height:160px;object-fit:cover;border-radius:10px;display:block;box-shadow:0 10px 26px rgba(0,0,0,0.08)}

    /* map */
    .map-wrap{margin-top:18px;border-radius:12px;overflow:hidden;border:1px solid rgba(123,31,162,0.06);box-shadow:0 12px 36px rgba(123,31,162,0.06)}

    /* footer */
    footer{margin-top:36px;padding:20px 0;text-align:center;color:var(--muted);border-top:1px solid rgba(123,31,162,0.04)}

    /* quick WA floating */
    .quick-wa{position:fixed;right:16px;bottom:16px;background:linear-gradient(90deg,var(--accent),var(--accent-2));color:#fff;padding:12px;border-radius:999px;box-shadow:0 12px 30px rgba(123,31,162,0.16);z-index:999}

    /* responsive */
    @media (max-width:1080px){
      .category-grid{grid-template-columns:repeat(2,1fr)}
      .testi-grid{grid-template-columns:repeat(2,1fr)}
      .gallery-grid{grid-template-columns:repeat(3,1fr)}
    }
    @media (max-width:720px){
      .wrap{padding:18px}
      .hero{min-height:44vh}
      .hero-inner{padding:36px 12px}
      .hero h2{font-size:1.9rem}
      .category-grid{grid-template-columns:1fr}
      .price-grid{grid-template-columns:1fr}
      .testi-grid{grid-template-columns:1fr}
      .gallery-grid{grid-template-columns:repeat(2,1fr)}
      .socials-large{flex-direction:column}
    }
    @media (max-width:420px){
      .gallery-grid{grid-template-columns:repeat(1,1fr)}
      .logo{width:52px;height:52px}
      .brand h1{font-size:1.05rem}
      .hero h2{font-size:1.6rem}
    }

    /* small accessibility helper */
    .sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border:0}
  </style>
</head>
<body>

  <div class="wrap" id="top">
    <!-- header -->
    <header>
      <div class="brand">
        <div class="logo">VB</div>
        <h1>Velin Beauty</h1>
      </div>

      <nav aria-label="Main navigation">
        <a href="#menu">Price List</a>
        <a href="#testimoni">Testimoni</a>
        <a href="#gallery">Gallery</a>
        <a href="#lokasi">Lokasi</a>
        <a class="btn-book" href="https://wa.me/6285785716869" target="_blank" rel="noopener">Booking via WA</a>
      </nav>
    </header>

    <!-- hero -->
    <section class="hero" aria-label="Hero">
      <div class="hero-inner">
        <h2>Velin Beauty Care & Spa</h2>
        <p>Perawatan premium & elegan — potong, smoothing, color, creambath, hair care & blow perm. Lihat daftar harga per kategori di bawah atau chat WA untuk konsultasi & booking.</p>
        <div class="cta-row">
          <a class="cta-ghost" href="#menu">Lihat Daftar Harga</a>
          <a class="cta-primary" href="https://wa.me/6285785716869?text=Halo%20Velin%20Beauty%2C%20saya%20ingin%20booking" target="_blank" rel="noopener">Booking via WhatsApp</a>
        </div>
      </div>
    </section>

    <!-- price list (per category) -->
    <section id="menu" class="section" aria-labelledby="price-title">
      <h2 class="title" id="price-title">PRICE LIST</h2>
      <p class="subtitle">Harga disajikan per kategori untuk memudahkan estimasi. Untuk hitungan final (panjang/tebal rambut atau warna khusus), harap chat WA dengan foto rambut.</p>

      <div class="category-grid" role="list">

        <!-- POTONG -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('potong.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">POTONG</h3>
            <p class="cat-desc">Layanan potong rambut — dari potong standar sampai paket lengkap dengan cuci & styling.</p>

   <style>
.price-list {
  max-width: 500px; /* sesuaikan dengan layout */
  margin: 0 auto;
  font-family: Arial, sans-serif;
}

.price-row {
  display: flex;
  justify-content: space-between; /* kiri-kanan */
  padding: 8px 0;
  border-bottom: 1px solid #ddd; /* optional garis bawah */
}

.price-left {
  text-align: left;
  font-weight: 500;
}

.price-right {
  text-align: right;
  font-weight: 600;
}
</style>

<style>
.price-list {
  max-width: 500px;
  margin: 0 auto;
  font-family: Arial, sans-serif;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

.price-row {
  display: flex;
  justify-content: space-between;
  padding: 12px 16px;
  transition: background 0.3s;
  font-variant-numeric: tabular-nums; /* angka rata kanan */
}

.price-row:nth-child(odd) {
  background-color: #f7f7f7;
}

.price-row:nth-child(even) {
  background-color: #ffffff;
}

.price-row:hover {
  background-color: #ffe6e6;
}

.price-left {
  text-align: left;
  font-weight: 500;
  flex: 1; /* kolom kiri fleksibel */
}

.price-right {
  text-align: right;
  font-weight: 600;
  color: #d63333;
  white-space: nowrap; /* supaya Rp dan angka tetap sebaris */
}
</style>

<style>
.price-list {
  max-width: 500px;
  margin: 0 auto;
  font-family: Arial, sans-serif;
  border-radius: 10px;
  overflow: hidden;
}

.price-row {
  display: flex;
  justify-content: space-between;
  padding: 12px 16px;
  transition: background 0.3s;
  font-variant-numeric: tabular-nums; /* angka rata */
  border-bottom: 1px solid #ccc; /* garis tipis pemisah */
  background-color: #f0f0f0; /* abu-abu terang */
}

.price-row:hover {
  background-color: #d9d9d9; /* abu-abu gelap saat hover */
}

.price-left {
  text-align: left;
  font-weight: 500;
  flex: 1;
}

.price-right {
  text-align: right;
  font-weight: 600;
  white-space: nowrap; /* Rp dan angka tetap sebaris */
}
</style>

<style>
.price-list {
  max-width: 500px;
  margin: 0 auto;
  font-family: Arial, sans-serif;
  border-radius: 10px;
  overflow: hidden;
}

.price-row {
  display: flex;
  justify-content: space-between;
  padding: 12px 16px;
  transition: background 0.3s;
  font-variant-numeric: tabular-nums; /* angka rata */
  border-bottom: 1px solid #ccc;
  background-color: #f0f0f0; /* abu-abu terang */
}

.price-row:hover {
  background-color: #d9d9d9; /* abu-abu gelap saat hover */
}

.price-left {
  text-align: left;
  font-weight: 500;
  flex: 1;
  color: #555; /* abu-abu untuk teks kiri */
}

.price-right {
  text-align: right;
  font-weight: 600;
  color: #555; /* abu-abu untuk harga juga */
  white-space: nowrap; /* Rp dan angka tetap sebaris */
}
</style>

<div class="price-list">
  <div class="price-row">
    <div class="price-left">Potong</div>
    <div class="price-right">Rp15.000 — Rp20.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Potong + Cuci + Vitamin</div>
    <div class="price-right">Rp30.000 — Rp40.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Potong + Catok</div>
    <div class="price-right">Rp30.000 — Rp35.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Potong + Cuci + Catok</div>
    <div class="price-right">Rp50.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Cuci Kering + Vitamin</div>
    <div class="price-right">Rp15.000 — Rp20.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Cuci + Catok / Curl + Vitamin</div>
    <div class="price-right">Rp35.000 — Rp40.000</div>
  </div>
</div>



            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20POTONG" target="_blank" rel="noopener">Pesan via WA</a>
              <div class="price-note">Estimasi & durasi konfirmasi via WA.</div>
            </div>
          </div>
        </article>

        <!-- SMOOTHING STANDARD -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('smoothingstandar.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">SMOOTHING — STANDARD</h3>
            <p class="cat-desc">Smoothing level standar: rambut lebih halus dan mudah diatur.</p>

   <style>
.price-list {
  max-width: 500px;
  margin: 0 auto;
  font-family: Arial, sans-serif;
  border-radius: 10px;
  overflow: hidden;
}

.price-row {
  display: flex;
  justify-content: space-between;
  padding: 12px 16px;
  border-bottom: 1px solid #ccc;
  background-color: #f0f0f0;
  transition: background 0.3s;
  font-variant-numeric: tabular-nums; /* angka rata */
}

.price-row:hover {
  background-color: #d9d9d9;
}

.price-left {
  flex: 1;
  text-align: left;
  font-weight: 500;
  color: #555;
}

.price-right {
  text-align: right;
  font-weight: 600;
  color: #555;
  white-space: nowrap; /* Rp dan angka tetap sebaris */
}
</style>

<div class="price-list">
  <div class="price-row">
    <div class="price-left">Pendek</div>
    <div class="price-right">Rp180.000 — Rp200.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Sedang</div>
    <div class="price-right">Rp200.000 — Rp250.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Panjang</div>
    <div class="price-right">Rp250.000 — Rp300.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Extra Tebal / Panjang</div>
    <div class="price-right">+ Rp30.000 — Rp50.000</div>
  </div>
</div>

            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20SMOOTHING%20STANDARD" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- SMOOTHING PREMIUM -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('smoothingpremium.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">SMOOTHING — PREMIUM</h3>
            <p class="cat-desc">Formula premium untuk hasil halus & daya tahan lebih lama.</p>

           <style>
.price-list {
  max-width: 500px;
  margin: 0 auto;
  font-family: Arial, sans-serif;
  border-radius: 10px;
  overflow: hidden;
}

.price-row {
  display: flex;
  justify-content: space-between;
  padding: 12px 16px;
  border-bottom: 1px solid #ccc;
  background-color: #f0f0f0;
  transition: background 0.3s;
  font-variant-numeric: tabular-nums; /* angka rata */
}

.price-row:hover {
  background-color: #d9d9d9;
}

.price-left {
  flex: 1;
  text-align: left;
  font-weight: 500;
  color: #555;
}

.price-right {
  text-align: right;
  font-weight: 600;
  color: #555;
  white-space: nowrap; /* Rp dan angka tetap sebaris */
}
</style>

<div class="price-list">
  <div class="price-row">
    <div class="price-left">Pendek</div>
    <div class="price-right">Rp200.000 — Rp250.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Sedang</div>
    <div class="price-right">Rp250.000 — Rp300.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Panjang</div>
    <div class="price-right">Rp300.000 — Rp350.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Extra Tebal / Panjang</div>
    <div class="price-right">+ Rp30.000 — Rp50.000</div>
  </div>
</div>


            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20SMOOTHING%20PREMIUM" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- SMOOTHING EXPRESS (SHOLEHAH) -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('smoothingsholehah.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">SMOOTHING — EXPRESS (SHOLEHAH)</h3>
            <p class="cat-desc">Pilihan ekspres dengan kualitas tetap terjaga.</p>

          <div class="price-list">
  <div class="price-row">
    <div class="price-left">Pendek</div>
    <div class="price-right">Rp190.000 — Rp230.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Sedang</div>
    <div class="price-right">Rp240.000 — Rp280.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Panjang</div>
    <div class="price-right">Rp290.000 — Rp320.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Extra Tebal / Panjang</div>
    <div class="price-right">+ Rp30.000 — Rp50.000</div>
  </div>
</div>


            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20SMOOTHING%20EXPRESS" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- SMOOTHING KERATIN JEPANG -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('smoothingjepang.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">SMOOTHING — KERATIN JEPANG</h3>
            <p class="cat-desc">Perawatan keratin teknik Jepang untuk hasil maksimal.</p>

          <div class="price-list">
  <div class="price-row">
    <div class="price-left">Pendek</div>
    <div class="price-right">Rp250.000 — Rp300.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Sedang</div>
    <div class="price-right">Rp300.000 — Rp350.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Panjang</div>
    <div class="price-right">Rp350.000 — Rp400.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Extra Tebal / Panjang</div>
    <div class="price-right">+ Rp50.000</div>
  </div>
</div>


            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20SMOOTHING%20KERATIN%20JEPANG" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- L'OREAL SMOOTHING -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('smoothingloreal.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">L'ORÉAL SMOOTHING</h3>
            <p class="cat-desc">Smoothing khusus L'Oréal untuk hasil premium.</p>

         <div class="price-list">
  <div class="price-row">
    <div class="price-left">Pendek</div>
    <div class="price-right">Rp250.000 — Rp300.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Sedang</div>
    <div class="price-right">Rp310.000 — Rp400.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Panjang</div>
    <div class="price-right">Rp400.000 — Rp500.000</div>
  </div>
</div>

            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20LOREAL%20SMOOTHING" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- SMOOTHING COLOUR -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('smoothingcolour.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">SMOOTHING + COLOUR</h3>
            <p class="cat-desc">Kombinasi smoothing dengan pewarnaan. Harga tergantung pemakaian & jenis warna.</p>

           <div class="price-list">
  <div class="price-row">
    <div class="price-left">Pendek</div>
    <div class="price-right">Rp300.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Sedang</div>
    <div class="price-right">Rp350.000 — Rp400.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Panjang</div>
    <div class="price-right">Rp400.000 — Rp500.000</div>
  </div>
</div>


            <div class="price-note">Catatan: Harga final tergantung jumlah & jenis warna (bleach/toner tambahan).</div>
            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20SMOOTHING%20COLOUR" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- CREMBATH BUAH -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('crembathbuah.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">CREMBATH BUAH</h3>
            <p class="cat-desc">Creambath berbasis buah untuk aroma menyegarkan dan nutrisi.</p>
<div class="price-list">
  <div class="price-row">
    <div class="price-left">Pendek</div>
    <div class="price-right">Rp40.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Sedang</div>
    <div class="price-right">Rp50.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Panjang</div>
    <div class="price-right">Rp70.000</div>
  </div>
</div>


            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20CREMBATH%20BUAH" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- CREMBATH INAURA -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('crembath1.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">CREMBATH INAURA</h3>
            <p class="cat-desc">Varian Inaura — lembut & menutrisi.</p>

           <div class="price-list">
  <div class="price-row">
    <div class="price-left">Pendek</div>
    <div class="price-right">Rp50.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Sedang</div>
    <div class="price-right">Rp70.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Panjang</div>
    <div class="price-right">Rp80.000</div>
  </div>
</div>


            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20CREMBATH%20INAURA" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- CREMBATH BUAH SENSORIA -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('crembath.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">CREMBATH BUAH — SENSORIA</h3>
            <p class="cat-desc">Varian Sensoria — aroma premium & nutrisi mendalam.</p>

            <div class="price-list">
              <div class="price-row"><div class="price-left">Creambath Sensoria</div><div class="price-right">Rp80.000 — Rp100.000</div></div>
            </div>

            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20CREMBATH%20SENSORIA" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- HAIR MASK -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('hairmask.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">HAIR MASK</h3>
            <p class="cat-desc">Masker profesional untuk berbagai kebutuhan rambut.</p>

           <div class="price-list">
  <div class="price-row">
    <div class="price-left">Keratin Pro</div>
    <div class="price-right">Rp50.000 — Rp80.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">Biolage</div>
    <div class="price-right">Rp60.000 — Rp90.000</div>
  </div>
  <div class="price-row">
    <div class="price-left">L'Oréal</div>
    <div class="price-right">Rp60.000 — Rp90.000</div>
  </div>
</div>


            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20HAIR%20MASK" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- HAIR SPA -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('spa.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">HAIR SPA</h3>
            <p class="cat-desc">Perawatan spa untuk kelembapan dan relaksasi rambut.</p>

            <div class="price-list">
              <div class="price-row"><div class="price-left">Hair Spa</div><div class="price-right">Rp50.000 — Rp80.000</div></div>
            </div>

            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20HAIR%20SPA" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- HAIR BOTOX -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('botox.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">HAIR BOTOX</h3>
            <p class="cat-desc">Perawatan intensif untuk perbaikan kerusakan & kilau instan.</p>

            <div class="price-list">
              <div class="price-row"><div class="price-left">Hair Botox</div><div class="price-right">Rp75.000 — Rp100.000</div></div>
            </div>

            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20HAIR%20BOTOX" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- TONING -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('toning.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">TONING</h3>
            <p class="cat-desc">Finishing warna & penyesuaian rona (pria & wanita).</p>

            <div class="price-list">
              <div class="price-row"><div class="price-left">Toning Pendek (Pria)</div><div class="price-right">Rp40.000 — Rp50.000</div></div>
              <div class="price-row"><div class="price-left">Toning Pendek (Bob)</div><div class="price-right">Rp50.000 — Rp80.000</div></div>
              <div class="price-row"><div class="price-left">Toning Sedang / Panjang</div><div class="price-right">Rp80.000 — Rp150.000</div></div>
            </div>

            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20TONING" target="_blank" rel="noopener">Pesan via WA</a>
            </div>
          </div>
        </article>

        <!-- WARNA BASIC -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('warna1.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">WARNA BASIC & HIGHLIGHT</h3>
            <p class="cat-desc">Warna dasar, highlight & bleaching. Foto referensi warna sangat disarankan.</p>

            <div class="price-list">
              <div class="price-row"><div class="price-left">Pendek (Basic)</div><div class="price-right">Rp70.000 — Rp100.000</div></div>
              <div class="price-row"><div class="price-left">Sedang (Basic)</div><div class="price-right">Rp100.000 — Rp120.000</div></div>
              <div class="price-row"><div class="price-left">Panjang (Basic)</div><div class="price-right">Rp120.000 — Rp150.000</div></div>
              <div class="price-row"><div class="price-left">Basic Premium</div><div class="price-right">Rp100.000 — Rp250.000</div></div>
              <div class="price-row"><div class="price-left">Highlight (Cowok)</div><div class="price-right">Rp75.000 — Rp150.000</div></div>
              <div class="price-row"><div class="price-left">Highlight (Cewek)</div><div class="price-right">Rp150.000 — Rp300.000</div></div>
              <div class="price-row"><div class="price-left">Bleaching Full</div><div class="price-right">Rp180.000 — Rp400.000</div></div>
            </div>

            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20WARNA%20BASIC" target="_blank" rel="noopener">Pesan via WA</a>
              <div class="price-note">Kirim foto & referensi warna via WA untuk estimasi bahan & harga final.</div>
            </div>
          </div>
        </article>

        <!-- BLOW PERM -->
        <article class="category-card" role="listitem">
          <div class="card-media" style="background-image:url('blow1.jpg')" aria-hidden="true"></div>
          <div class="card-body">
            <h3 class="cat-title">BLOW PERM</h3>
            <p class="cat-desc">Teknik blow perm untuk perubahan tekstur & volume. Harga tergantung teknik & panjang rambut.</p>

            <div class="price-list">
              <div class="price-row"><div class="price-left">Blow Perm</div><div class="price-right">Rp250.000 — Rp500.000</div></div>
            </div>

            <div class="card-footer">
              <a class="btn-wa" href="https://wa.me/6285785716869?text=Booking%20BLOW%20PERM" target="_blank" rel="noopener">Pesan via WA</a>
              <div class="price-note">Harga final akan dikonfirmasi setelah konsultasi & pengecekan rambut.</div>
            </div>
          </div>
        </article>

      </div> <!-- /category-grid -->
    </section>

    <!-- testimonials -->
    <section id="testimoni" class="section" aria-labelledby="testi-title">
      <h2 class="title" id="testi-title">Testimoni Klien</h2>
      <p class="subtitle">Pengalaman nyata dari pelanggan kami.</p>

      <div class="testi-grid">
        <div class="testi-card"><p>"Pelayanan ramah, hasil smoothing awet dan rambut jadi lembut."</p><div class="testi-author">— Rina</div></div>
        <div class="testi-card"><p>"Potongan sesuai referensi, stylist telaten."</p><div class="testi-author">— Dinda</div></div>
        <div class="testi-card"><p>"Creambathnya wangi dan bikin rambut halus. Tempatnya bersih."</p><div class="testi-author">— Maya</div></div>
      </div>
    </section>

 <!-- gallery -->
<section id="gallery" class="section" aria-labelledby="gallery-title">
  <h2 class="title" id="gallery-title">Gallery Client</h2>
  <p class="subtitle">Foto hasil perawatan & contoh styling. (Ganti dengan foto asli salon untuk hasil lebih personal)</p>

  <div class="gallery-grid">
    <!-- Haircut -->
    <img src="https://images.unsplash.com/photo-1611434003449-479f94932b17?auto=format&fit=crop&w=1200&q=80" alt="Haircut client" loading="lazy">
    <!-- Hair coloring -->
    <img src="https://images.unsplash.com/photo-1614622701498-c3dc6d2c7282?auto=format&fit=crop&w=1200&q=80" alt="Hair coloring client" loading="lazy">
    <!-- Hair styling -->
    <img src="https://images.unsplash.com/photo-1611605690624-4f0caa5c9d60?auto=format&fit=crop&w=1200&q=80" alt="Hair styling client" loading="lazy">
    <!-- Spa treatment -->
    <img src="https://images.unsplash.com/photo-1580281657525-29cd93b3b0d7?auto=format&fit=crop&w=1200&q=80" alt="Spa treatment" loading="lazy">
    <!-- Blow dry -->
    <img src="https://images.unsplash.com/photo-1611638355166-79d9c2179f5e?auto=format&fit=crop&w=1200&q=80" alt="Blow dry" loading="lazy">
    <!-- Hair mask -->
    <img src="https://images.unsplash.com/photo-1611605262017-2c7b4de0b346?auto=format&fit=crop&w=1200&q=80" alt="Hair mask treatment" loading="lazy">
    <!-- Premium smoothing -->
    <img src="https://images.unsplash.com/photo-1611639243211-c6b95c0e4d8f?auto=format&fit=crop&w=1200&q=80" alt="Premium smoothing" loading="lazy">
    <!-- Salon interior -->
    <img src="https://images.unsplash.com/photo-1603920941650-3f1a16047a2f?auto=format&fit=crop&w=1200&q=80" alt="Salon interior" loading="lazy">
  </div>
</section>


    <!-- socials large above map + map embed -->
    <section id="lokasi" class="section" aria-labelledby="lokasi-title">
      <h2 class="title" id="lokasi-title">Sosial Media & Lokasi</h2>
      <p class="subtitle">Klik tombol untuk membuka profil sosial atau chat WA. Peta di bawah menunjukkan lokasi salon (embed & link aktif).</p>

      <div class="socials-large" role="navigation" aria-label="Sosial Media Utama">
        <a class="social-card" href="https://www.instagram.com/velinsalon_beautyspa?igsh=MXdhNXZ3MWI0Mms3cQ==" target="_blank" rel="noopener">
          <img src="https://cdn-icons-png.flaticon.com/512/174/174855.png" alt="Instagram icon">
          <div class="info">
            <div class="label">Instagram</div>
            <div class="meta">@velinsalon_beautyspa</div>
            <div class="action">Buka Instagram</div>
          </div>
        </a>

        <a class="social-card" href="https://www.tiktok.com/@velinsalon?_t=ZS-8zRL8UlFBRJ&_r=1" target="_blank" rel="noopener">
          <img src="https://cdn-icons-png.flaticon.com/512/3046/3046127.png" alt="TikTok icon">
          <div class="info">
            <div class="label">TikTok</div>
            <div class="meta">@velinsalon</div>
            <div class="action">Buka TikTok</div>
          </div>
        </a>

        <a class="social-card" href="https://wa.me/6285785716869" target="_blank" rel="noopener">
          <img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" alt="WhatsApp icon">
          <div class="info">
            <div class="label">WhatsApp</div>
            <div class="meta">+62 857-8571-6869</div>
            <div class="action">Chat WhatsApp</div>
          </div>
        </a>
      </div>

      <div class="map-wrap" aria-hidden="false" style="margin-top:18px;">
        <!-- USER-SUPPLIED EMBED - used as-is for accuracy -->
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1541351.7362811477!2d109.31263079375!3d-7.8758136000000025!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e79a7fc9f5f19af%3A0x292b3554a84d480e!2sVelin%20Salon%202!5e1!3m2!1sid!2sid!4v1756970540564!5m2!1sid!2sid"
          width="100%" height="420" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade">
        </iframe>
      </div>

      <p style="text-align:center;margin-top:12px"><a href="https://maps.app.goo.gl/Y9b8ofBXXej2GxXp7" target="_blank" rel="noopener" style="color:var(--accent-2);font-weight:700">Buka di Google Maps</a></p>
    </section>

    <!-- footer -->
   <footer>

    <div class="footer-right">
      <div>&copy; 2025 Velin Beauty Care & Spa</div>
      <div class="footer-socials">
        <a href="https://www.instagram.com/velinsalon_beautyspa" target="_blank" rel="noopener">Instagram</a> ·
        <a href="https://www.tiktok.com/@velinsalon" target="_blank" rel="noopener">TikTok</a> ·
        <a href="https://wa.me/6285785716869" target="_blank" rel="noopener">WhatsApp</a>
      </div>
    </div>
  </div>
</footer>


  </div> <!-- /wrap -->

  <!-- quick WA floating -->
  <a class="quick-wa" href="https://wa.me/6285785716869" target="_blank" rel="noopener" aria-label="Chat WhatsApp">
    Chat / Booking — +62 857-8571-6869
  </a>

  <script>
    // Smooth scroll for in-page anchor links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        const target = document.querySelector(a.getAttribute('href'));
        if(target){
          e.preventDefault();
          target.scrollIntoView({behavior:'smooth',block:'start'});
        }
      });
    });

    // lazy load gallery images (improve performance)
    document.querySelectorAll('.gallery-grid img').forEach(img => img.loading = 'lazy');
  </script>
</body>
</html>
