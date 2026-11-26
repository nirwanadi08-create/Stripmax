<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>STRIPMAX - Penghapus Emulsi Sablon</title>
  <style>
    :root {
      --bg: #111317;
      --card: #1a1d24;
      --card-2: #222630;
      --text: #f5f7fa;
      --muted: #b0b7c3;
      --accent: #f59e0b;
      --accent-dark: #d97706;
      --wa: #22c55e;
      --wa-dark: #16a34a;
      --border: #2e3440;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.5;
      padding-bottom: 84px;
    }

    .topbar {
      background: #ea580c;
      color: #ffffff;
      text-align: center;
      font-size: 13px;
      font-weight: 700;
      padding: 9px 12px;
      letter-spacing: 0.2px;
    }

    .container {
      max-width: 520px;
      margin: 0 auto;
      padding: 18px 16px;
    }

    .badge {
      display: inline-block;
      background: rgba(245, 158, 11, 0.14);
      border: 1px solid rgba(245, 158, 11, 0.45);
      color: #fbbf24;
      font-size: 12px;
      font-weight: 700;
      padding: 5px 10px;
      border-radius: 999px;
      margin-bottom: 12px;
      letter-spacing: 0.5px;
    }

    h1 {
      font-size: 26px;
      line-height: 1.25;
      margin-bottom: 10px;
      font-weight: 800;
    }

    h1 span {
      color: #fbbf24;
    }

    .sub {
      color: var(--muted);
      font-size: 15px;
      margin-bottom: 18px;
    }

    .product-box {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 14px;
      padding: 12px;
      margin-bottom: 18px;
      text-align: center;
    }

    .product-box img {
      width: 100%;
      max-height: 360px;
      object-fit: cover;
      border-radius: 10px;
      display: block;
      margin-bottom: 10px;
    }

    .product-caption {
      font-size: 13px;
      color: #e5e7eb;
      font-weight: 600;
    }

    .btn-wa {
      display: block;
      width: 100%;
      background: var(--wa);
      color: #08130b;
      text-decoration: none;
      text-align: center;
      font-weight: 800;
      font-size: 15px;
      padding: 14px 16px;
      border-radius: 10px;
      border: none;
      cursor: pointer;
      transition: background 0.2s ease;
    }

    .btn-wa:hover {
      background: var(--wa-dark);
      color: #ffffff;
    }

    .section-title {
      font-size: 18px;
      font-weight: 800;
      margin: 22px 0 12px;
    }

    .benefits {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 14px;
      padding: 14px 16px;
      list-style: none;
    }

    .benefits li {
      padding: 7px 0;
      border-bottom: 1px solid var(--border);
      font-size: 14px;
      color: #e5e7eb;
    }

    .benefits li:last-child {
      border-bottom: none;
    }

    .packages {
      display: grid;
      gap: 12px;
    }

    .pkg {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 14px;
      padding: 14px 16px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
      cursor: pointer;
    }

    .pkg.active {
      border-color: var(--accent);
      background: var(--card-2);
    }

    .pkg-name {
      font-weight: 700;
      font-size: 15px;
    }

    .pkg-desc {
      font-size: 12.5px;
      color: var(--muted);
      margin-top: 2px;
    }

    .pkg-price {
      font-weight: 800;
      font-size: 16px;
      color: #fbbf24;
      white-space: nowrap;
    }

    .form-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 14px;
      padding: 16px;
      margin-top: 14px;
    }

    .field {
      margin-bottom: 12px;
    }

    label {
      display: block;
      font-size: 13px;
      font-weight: 600;
      margin-bottom: 5px;
      color: #e5e7eb;
    }

    input, select {
      width: 100%;
      padding: 11px 12px;
      border-radius: 9px;
      border: 1px solid var(--border);
      background: #111317;
      color: var(--text);
      font-size: 14px;
    }

    input:focus, select:focus {
      outline: none;
      border-color: var(--accent);
    }

    .sticky-bar {
      position: fixed;
      left: 0;
      right: 0;
      bottom: 0;
      background: rgba(17, 19, 23, 0.96);
      border-top: 1px solid var(--border);
      padding: 10px 14px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      z-index: 99;
    }

    .sticky-price-label {
      font-size: 11.5px;
      color: var(--muted);
    }

    .sticky-price-val {
      font-size: 16px;
      font-weight: 800;
      color: #fbbf24;
    }

    .sticky-btn {
      background: var(--wa);
      color: #08130b;
      text-decoration: none;
      font-weight: 800;
      font-size: 14px;
      padding: 11px 16px;
      border-radius: 9px;
      white-space: nowrap;
    }
  </style>
</head>
<body>
  <div class="topbar">
    PROMO KHUSUS BENGKEL SABLON — BISA COD BAYAR DI TEMPAT!
  </div>

  <div class="container">
    <div class="badge">STRIPMAX • EMULSION REMOVER</div>
    <h1>Rontokkan Obat Afdruk Membandel <span>Dalam Hitungan Menit</span> Tanpa Merusak Mesh!</h1>
    <p class="sub">
      Formula pasta pekat khusus tukang sablon. Oles, diamkan sebentar, semprot air — screen langsung bersih siap afdruk ulang.
    </p>

    <div class="product-box">
      <img
        src="produk.jpg"
        alt="Foto Produk Stripmax Penghapus Emulsi Sablon"
        onerror="this.style.display='none';"
      />
      <div class="product-caption">
        Pasta pekat siap pakai — hemat pemakaian untuk kebutuhan harian bengkel sablon
      </div>
    </div>

    <a
      id="directWaBtn"
      class="btn-wa"
      href="https://wa.me/6282245800129?text=Halo%20Admin%20Stripmax%2C%20saya%20mau%20tanya%20%26%20pesan%20Penghapus%20Emulsi%20Sablon%20Stripmax."
      target="_blank"
      rel="noopener"
    >
      AMBIL PROMO &amp; PESAN VIA WHATSAPP &rarr;
    </a>

    <h2 class="section-title">Kenapa Banyak Tukang Sablon Pakai Stripmax?</h2>
    <ul class="benefits">
      <li><strong>Tekstur pasta pekat</strong> — tidak gampang meleleh sebelum sempat bekerja di screen.</li>
      <li><strong>Cepat melunakkan afdruk</strong> — bantu hemat waktu bersihkan screen saat kejar order.</li>
      <li><strong>Aman untuk kain/mesh</strong> — tidak bikin kain cepat rapuh bila dipakai sesuai takaran.</li>
      <li><strong>Bisa COD</strong> — cek barang saat sampai (sesuai jangkauan kurir).</li>
    </ul>

    <h2 class="section-title">Pilih Paket Hemat</h2>
    <div class="packages">
      <div class="pkg active" data-pkg="Paket Coba (Rp35.000)" onclick="selectPkg(this)">
        <div>
          <div class="pkg-name">Paket Coba</div>
          <div class="pkg-desc">Cocok untuk tes hasil di bengkel sendiri</div>
        </div>
        <div class="pkg-price">Rp 35.000</div>
      </div>

      <div class="pkg" data-pkg="Paket Bengkel (Rp60.000)" onclick="selectPkg(this)">
        <div>
          <div class="pkg-name">Paket Bengkel</div>
          <div class="pkg-desc">Paling laris untuk produksi rutin harian</div>
        </div>
        <div class="pkg-price">Rp 60.000</div>
      </div>

      <div class="pkg" data-pkg="Paket Juragan (Rp105.000)" onclick="selectPkg(this)">
        <div>
          <div class="pkg-name">Paket Juragan</div>
          <div class="pkg-desc">Stok lebih banyak, harga makin hemat</div>
        </div>
        <div class="pkg-price">Rp 105.000</div>
      </div>
    </div>

    <div class="form-card">
      <div class="field">
        <label for="nama">Nama Anda</label>
        <input type="text" id="nama" placeholder="Contoh: Mas Adi / Bengkel Sablon Jaya" />
      </div>

      <div class="field">
        <label for="paket">Paket Dipilih</label>
        <select id="paket" onchange="syncPkgFromSelect()">
          <option value="Paket Coba (Rp35.000)" selected>Paket Coba — Rp 35.000</option>
          <option value="Paket Bengkel (Rp60.000)">Paket Bengkel — Rp 60.000</option>
          <option value="Paket Juragan (Rp105.000)">Paket Juragan — Rp 105.000</option>
        </select>
      </div>

      <div class="field">
        <label for="kota">Kota / Kecamatan Tujuan</label>
        <input type="text" id="kota" placeholder="Contoh: Bojonegoro / Madiun" />
      </div>

      <button type="button" class="btn-wa" onclick="kirimWA()">
        KIRIM ORDER KE WHATSAPP SEKARANG &rarr;
      </button>
    </div>
  </div>

  <div class="sticky-bar">
    <div>
      <div class="sticky-price-label">Harga Promo Mulai</div>
      <div class="sticky-price-val">Rp 35.000</div>
    </div>
    <a
      class="sticky-btn"
      href="https://wa.me/6282245800129?text=Halo%20Admin%20Stripmax%2C%20saya%20mau%20pesan%20Penghapus%20Emulsi%20Sablon%20Stripmax."
      target="_blank"
      rel="noopener"
    >
      Pesan Sekarang &rarr;
    </a>
  </div>

  <script>
    function selectPkg(el) {
      document.querySelectorAll(".pkg").forEach(function (item) {
        item.classList.remove("active");
      });
      el.classList.add("active");
      document.getElementById("paket").value = el.getAttribute("data-pkg");
    }

    function syncPkgFromSelect() {
      var val = document.getElementById("paket").value;
      document.querySelectorAll(".pkg").forEach(function (item) {
        item.classList.toggle("active", item.getAttribute("data-pkg") === val);
      });
    }

    function kirimWA() {
      var nama = document.getElementById("nama").value.trim() || "-";
      var paket = document.getElementById("paket").value;
      var kota = document.getElementById("kota").value.trim() || "-";

      var pesan =
        "Halo Admin Stripmax, saya mau order Penghapus Emulsi Sablon Stripmax.%0A" +
        "Nama: " + encodeURIComponent(nama) + "%0A" +
        "Paket: " + encodeURIComponent(paket) + "%0A" +
        "Kota/Kecamatan: " + encodeURIComponent(kota);

      window.open("https://wa.me/6282245800129?text=" + pesan, "_blank", "noopener");
    }
  </script>
</body>
</html>
