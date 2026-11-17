# Game Simulasi Agronomi Jagung

Lima game kecil untuk belajar budidaya dan produksi benih jagung. Gratis, langsung dimainkan di browser, tanpa instalasi.

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

## Roguing Challenge

Game ketuk cepat membuang tanaman menyimpang di pertanaman benih. Empat baris jagung (dua betina, dua jantan) bergerak dari kiri ke kanan, dan pemain harus mencabut tanaman yang salah sebelum lolos:

- **Off type (simpang):** batang agak merah, lebih tinggi, daun lebih pucat. Bisa muncul di semua baris.
- **PCO (kerdil):** tanaman pendek, hanya muncul di baris betina.
- **Volunteer:** tanaman sisa jagung musim sebelumnya, hanya muncul di lahan bekas jagung.

Jantan (hijau terang) dan betina (hijau gelap) yang normal harus dibiarkan. Di awal pemain memilih **lahan baru** atau **bekas jagung**, dan menu awal menampilkan gambar tiap jenis tanaman. Waktu 60 detik: salah cabut mengurangi waktu, tanaman salah yang lolos mengurangi poin, dan cabutan beruntun memberi bonus combo. Dilengkapi efek suara.

Main: https://meer-sa.github.io/Simulasi-Jagung/roguing-challenge/

## Menyiangi Gulma

Game ketuk cepat membedakan jagung dari gulma. Cabut gulma sebelum menguasai petak, tanpa salah mencabut jagung yang berpindah-pindah petak:

- **Gulma daun sempit (rumput):** helai tipis, merumpun, hijau muda. Mirip jagung muda tetapi jauh lebih kecil.
- **Gulma daun lebar:** daun bulat telur, batang kemerahan, berbunga saat sudah besar.
- **Teki:** daun lurus mengilap hijau tua, berumbi. Harus diketuk dua kali agar umbinya ikut tercabut.

Menu awal menampilkan gambar dan ciri tiap tanaman, termasuk jagung. Waktu 60 detik: gulma tumbuh dalam tiga stadia dan yang dibiarkan besar menurunkan hasil panen tiap detik, jadi gulma kecil bernilai lebih banyak. Salah cabut jagung mengurangi skor dan hasil panen, cabutan beruntun memberi bonus combo, dan tingkat kesulitan naik setiap 10 detik (gulma muncul dan tumbuh lebih cepat, jagung lebih sering berpindah). Dilengkapi efek suara.

Main: https://meer-sa.github.io/Simulasi-Jagung/menyiangi-gulma/

## Struktur repo

```
.
├── index.html            menu utama
├── README.md
├── petak-jagung/index.html
├── pembasmi-hama/index.html
├── detasseling-rush/index.html
├── roguing-challenge/index.html
└── menyiangi-gulma/index.html
```

## Catatan

- Skor terbaik disimpan di browser pemain (localStorage), bukan di server.
- Koneksi internet hanya dipakai untuk memuat font Google. Tanpa internet, game tetap jalan dengan font bawaan.
- Roguing Challenge dan Menyiangi Gulma membuat efek suaranya langsung di browser, jadi suara baru aktif setelah pemain mengetuk tombol Mulai. Roguing Challenge punya tombol 🔊 di layar game untuk mematikan suara, sedangkan Menyiangi Gulma punya tombol Suara nyala/mati di pojok kanan atas.

## Masukan

Terbuka untuk saran dan koreksi, terutama dari rekan agronomis. Silakan buka Issues di repo ini.
