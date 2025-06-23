<style>
  body {
    background-color: #3b2f1e; /* dark gold background */
    color: white;
    font-family: 'Segoe UI', sans-serif;
    padding: 20px;
  }

  h2, h3 {
    color: #FFD700; /* gold text */
  }

  input, select, button {
    width: 100%;
    padding: 10px;
    margin-bottom: 15px;
    border-radius: 8px;
    border: none;
    font-size: 16px;
  }

  input, select {
    background-color: #fffbe6;
    color: #000;
  }

  button {
    background-color: #FFD700;
    color: #000;
    font-weight: bold;
    cursor: pointer;
  }

  button:hover {
    background-color: #e6c200;
  }
</style>

<h2>🛒 MAZZ ALDI STORE</h2>
<p>Silakan isi data dan pilih layanan kamu:</p>

<label>Nama Pelanggan:</label>
<input type="text" id="nama" placeholder="Masukkan Nama Kamu">

<label>Pilih Layanan:</label>
<select id="layanan">
  <option value="Top Up FF">Top Up Diamond Free Fire</option>
  <option value="Suntik Followers TikTok">Suntik Followers TikTok</option>
  <option value="Suntik Followers IG">Suntik Followers Instagram</option>
  <option value="Like TikTok">Like TikTok</option>
  <option value="Like Instagram">Like Instagram</option>
  <option value="Pengikut Saluran WA">Pengikut Saluran WhatsApp</option>
</select>

<label>Pilih Paket:</label>
<select id="paket">
  <!-- FF -->
  <option value="FF 100 DM = 13.427">FF 100 DM = 13.427</option>
  <option value="FF 200 DM = 26.577">FF 200 DM = 26.577</option>
  <option value="FF 500 DM = 64.630">FF 500 DM = 64.630</option>

  <!-- TikTok Followers -->
  <option value="TikTok 100 Foll = 3,5K">TikTok 100 Foll = 3,5K</option>
  <option value="TikTok 500 Foll = 13K">TikTok 500 Foll = 13K</option>

  <!-- IG Followers -->
  <option value="IG 100 Followers = 2,5K">IG 100 Followers = 2,5K</option>
  <option value="IG 500 Followers = 9K">IG 500 Followers = 9K</option>

  <!-- Like TikTok -->
  <option value="Like TikTok 100 = 1K">Like TikTok 100 = 1K</option>
  <option value="Like TikTok 1000 = 7K">Like TikTok 1000 = 7K</option>

  <!-- Like IG -->
  <option value="Like IG 100 = 500P">Like IG 100 = 500P</option>
  <option value="Like IG 500 = 2,5K">Like IG 500 = 2,5K</option>

  <!-- WA Saluran -->
  <option value="Pengikut WA 10 = 500P">Pengikut WA 10 = 500P</option>
  <option value="Pengikut WA 100 = 5K">Pengikut WA 100 = 5K</option>
</select>

<button onclick="kirimPesanan()">📲 Kirim Pesanan ke WhatsApp</button>

<script>
function kirimPesanan() {
  const nama = document.getElementById("nama").value;
  const layanan = document.getElementById("layanan").value;
  const paket = document.getElementById("paket").value;
  const noAdmin = "6285705647386";

  const pesan = `Halo Admin MAZZ ALDI STORE!%0ASaya ingin pesan:%0A🧑 Nama: ${nama}%0A📌 Layanan: ${layanan}%0A📦 Paket: ${paket}`;

  window.open(`https://wa.me/${noAdmin}?text=${pesan}`, "_blank");
}
</script>
