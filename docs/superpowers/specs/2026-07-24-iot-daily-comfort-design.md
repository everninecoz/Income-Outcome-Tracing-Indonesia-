# Rancangan Penyempurnaan Pengalaman Harian IOT

## Tujuan

Membuat IOT terasa lebih ringan, cepat, dan nyaman dipakai setiap hari—baik dari desktop maupun ponsel—tanpa mengubah struktur data Supabase atau memecah aplikasi dari `iot.html`.

## Ruang lingkup

- Menata ulang dashboard agar saldo dan input transaksi langsung terlihat.
- Merapikan filter, riwayat transaksi, menu, dan modal agar lebih enak digunakan di layar kecil.
- Membuat pesan setelah input, status simpan, fokus keyboard, dan cara menutup panel terasa lebih jelas.
- Merapikan bagian CSS dan JavaScript yang disentuh lewat komentar internal, tanpa membuat file baru.
- Memperbarui versi aplikasi serta catatan perubahan singkat di README GitHub.

## Desain antarmuka

Bagian atas akan menempatkan saldo utama, input cepat, dan konteks periode saat ini dalam urutan yang lebih mudah dipindai. Di layar kecil, filter transaksi dibuat lebih ringkas. Daftar transaksi diberi jarak, kontras, dan tombol aksi yang lebih nyaman disentuh. Menu hanya menampilkan aksi penting agar layar tidak terasa ramai.

Dark mode tetap menjadi tampilan awal dan mode terang tetap tersedia. Semua permukaan input menggunakan token warna yang konsisten pada kedua tema.

## Interaksi dan aksesibilitas

Setiap panel atau modal bisa dibuka dengan keyboard, ditutup memakai Escape atau klik di luar panel, lalu mengembalikan fokus ke tombol pembukanya. Pesan transaksi akan muncul dekat area input, sedangkan status simpan tetap mudah terlihat tanpa mengganggu susunan halaman.

## Data dan kompatibilitas

Nama key, bentuk data akun, transaksi, anggaran, target, pengaturan, dan format backup tidak berubah. Tahap ini hanya menyentuh tampilan dan cara berinteraksi; alur penyimpanan Supabase yang sekarang tetap digunakan.

## Verifikasi

- Uji statis untuk struktur modal, tombol, dan token tema.
- Pemeriksaan manual desktop dan lebar 375 px bila browser tersedia.
- Uji input transaksi, filter, buka/tutup modal, mode terang/gelap, serta ekspor/impor.
- Pastikan versi aplikasi dan README diperbarui.
