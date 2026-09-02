# Kalkulator Interior Mobile V5.5

Versi ini memperbaiki logika kombinasi **WPC + Wallboard + UV Marble** menjadi komposisi bertingkat:

1. UV Marble menjadi aksen di tengah.
2. UV **mengambil/memotong area dari bidang Wallboard**, bukan ditambahkan di luar area Wallboard.
3. Sisa Wallboard menjadi bingkai di kiri-kanan UV dan, bila tinggi UV lebih pendek dari dinding, juga di atas-bawah UV.
4. WPC menjadi material paling luar di sisi kanan-kiri.
5. Luas WPC + Wallboard tersisa + UV selalu kembali ke luas dinding total, sehingga tidak ada double count.
6. Potongan WPC dan Wallboard dioptimalkan dari stok panjang yang ada.

## Contoh 3 × 3 m
Tipe Wallboard 40 cm dan UV 1,2 × 2,4 m:
- UV: 1 bidang, lebar 1,2 m, tinggi 2,4 m.
- Wallboard: bingkai 0,4 m di kiri dan kanan UV + ±0,3 m di atas dan bawah UV.
- WPC: sisa luar ±0,5 m di kiri dan kanan dinding.
- Area: WPC 3,00 m² + Wallboard 3,12 m² + UV 2,88 m² = 9,00 m².
- Estimasi dasar: WPC 8 keping, Wallboard 3 keping, UV 1 lembar (sebelum perubahan harga/asumsi oleh pengguna).

## Upload ke Vercel
Upload seluruh isi folder ini sebagai static site. File utama adalah `index.html`.
