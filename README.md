# Petak Jagung

Game simulasi budidaya jagung 1 hektar selama 110 HST. Pemain mengatur pemupukan (Urea, SP-36, KCl, NPK), irigasi, penyiangan, serta pengendalian ulat grayak, penggerek batang, tikus, bulai, dan hawar daun, sambil menghadapi cuaca yang berubah. Di akhir ada hasil panen, laba bersih, dan rincian penyebab kehilangan hasil.

Seluruh game ada dalam **satu file: `index.html`**. Tidak perlu instalasi, build, atau server. Cukup dibuka di browser.

> Model disederhanakan untuk belajar. Harga dan respons hara hanya contoh, bukan rekomendasi dosis lapangan.

## Mencoba di komputer sendiri

Klik dua kali `index.html`. Koneksi internet hanya dipakai untuk memuat font Google. Tanpa internet game tetap jalan dengan font bawaan.

## Menaruh di GitHub Pages (gratis, tanpa command line)

1. Masuk ke github.com, klik **New repository**, beri nama misalnya `petak-jagung`, pilih **Public**, lalu **Create repository**.
2. Di halaman repo, klik **uploading an existing file**, tarik `index.html` dan `README.md` ke sana, lalu klik **Commit changes**.
3. Buka **Settings → Pages**. Pada **Build and deployment**, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu **Save**.
4. Tunggu 1 sampai 2 menit. Alamatnya akan muncul di halaman yang sama, bentuknya `https://NAMA-GITHUB-KAMU.github.io/petak-jagung/`. Bagikan alamat itu ke siapa saja.

## Cara memperbarui

**Lewat web GitHub:**
1. Buka repo, klik `index.html`, lalu klik ikon pensil (**Edit this file**).
2. Ubah isinya, klik **Commit changes**.
3. Situs ikut diperbarui dalam 1 sampai 2 menit. Kalau tampilan lama masih muncul, muat ulang dengan Ctrl+F5 atau Cmd+Shift+R.

**Lewat Git di komputer:**
```bash
git add index.html
git commit -m "Perbaiki keseimbangan hasil panen"
git push
```

Setiap kali mengubah sesuatu yang berarti, ganti nomor versi di bagian bawah `index.html` (cari `Petak Jagung v1.1`).

## Alternatif tempat unggah

- **Netlify Drop**: buka app.netlify.com/drop, tarik folder berisi `index.html`. Langsung dapat alamat. Untuk memperbarui, tarik folder lagi pada situs yang sama.
- **Cloudflare Pages** atau **Vercel**: hubungkan repo GitHub tadi, tanpa perintah build, folder output `/`.
- **Hosting biasa**: unggah `index.html` ke folder publik.

## Di mana mengubah angka

Cari bagian `ENGINE_START` di dalam `index.html`. Semua angka keseimbangan ada di sana.

| Mau mengubah | Cari |
| --- | --- |
| Lama musim tanam | `DAYS` |
| Potensi hasil (t/ha) | `YMAX` |
| Kebutuhan N, P, K per musim | `REQ` |
| Harga jagung dan pupuk | `PRICE` |
| Biaya irigasi, siang, semprot, tikus | `COSTS` |
| Fase pertumbuhan dan saran | `STAGES` |
| Cara cuaca dibuat | `genWeather` |
| Aturan harian (air, hara, hama, penyakit, tikus) | `stepDay` |
| Efek dosis pupuk | `fertGain` |

Bagian bawah file (`UI`) berisi tampilan dan tombol.

## Catatan

- Cuaca dibuat acak setiap permainan. Tombol "Ulang dengan cuaca yang sama" memakai cuaca yang sama persis agar strategi bisa dibandingkan.
- Rekor laba disimpan di browser pemain (localStorage), bukan di server.
