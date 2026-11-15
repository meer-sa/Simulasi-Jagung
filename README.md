# Game Simulasi Agronomi Jagung

Tiga game kecil untuk belajar budidaya dan produksi benih jagung. Gratis, langsung dimainkan di browser, tanpa instalasi.

> Masih tahap pengembangan. Angka harga, biaya, dan respons tanaman hanya contoh yang disederhanakan, bukan rekomendasi. Pilihan bahan aktif juga disederhanakan dan belum divalidasi terhadap label produk atau peraturan, jadi selalu ikuti label dan anjuran setempat.

Menu utama: https://meer-sa.github.io/Simulasi-Jagung/

## Petak Jagung

Kelola 1 hektar jagung selama 110 hari: atur pupuk, irigasi, penyiangan, hama, tikus, dan penyakit di tengah cuaca yang berubah. Di akhir ada hasil panen, laba, dan rincian penyebab kehilangan hasil.

Main: https://meer-sa.github.io/Simulasi-Jagung/petak-jagung/

## Pembasmi Hama

Ketuk hama atau penyakit yang muncul di tanaman, lalu pilih bahan aktif atau penanganan yang tepat sebelum waktunya habis. Ada 14 hama dan penyakit, pilihan waktu 15, 30, atau 60 detik, mode ahli, dan kamus hama.

Main: https://meer-sa.github.io/Simulasi-Jagung/pembasmi-hama/

## Detasseling Rush

Game ketuk cepat produksi benih hibrida: cabut tassel tanaman betina sebelum melepas serbuk sari, dan biarkan baris jantan. Salah cabut atau terlambat menurunkan mutu benih. Pilihan waktu 15, 30, atau 60 detik.

Main: https://meer-sa.github.io/Simulasi-Jagung/detasseling-rush/

## Struktur repo

```
.
├── index.html            menu utama
├── README.md
├── petak-jagung/index.html
├── pembasmi-hama/index.html
└── detasseling-rush/index.html
```

## Memperbarui

1. Buka folder game yang mau diubah, misalnya `pembasmi-hama`.
2. Ketuk **Add file**, pilih **Upload files**, lalu unggah file versi baru dengan nama **`index.html`** agar file lama tertimpa.
3. Ketuk **Commit changes**. Situs ikut diperbarui dalam 1 sampai 2 menit. Kalau tampilan lama masih muncul, muat ulang atau buka lewat tab privat.

## Catatan

- Skor terbaik disimpan di browser pemain (localStorage), bukan di server.
- Koneksi internet hanya dipakai untuk memuat font Google. Tanpa internet, game tetap jalan dengan font bawaan.

## Masukan

Terbuka untuk saran dan koreksi, terutama dari rekan agronomis. Silakan buka Issues di repo ini.
