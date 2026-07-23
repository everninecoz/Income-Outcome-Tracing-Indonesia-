# Rancangan Kenyamanan Harian IOT

## Tujuan

Membuat penggunaan harian IOT lebih cepat, tenang, dan nyaman di desktop maupun ponsel tanpa mengubah struktur data Supabase atau memecah aplikasi dari `iot.html`.

## Ruang lingkup

- Menata ulang hirarki visual dashboard agar saldo dan input transaksi menjadi fokus utama.
- Merapikan filter, riwayat transaksi, menu, serta modal untuk layar kecil dan target sentuh yang lebih mudah.
- Memperjelas feedback input, status simpan, fokus keyboard, dan penutupan overlay.
- Mengelompokkan CSS dan JavaScript yang disentuh dengan komentar internal, tanpa memindahkan ke file lain.
- Menaikkan versi aplikasi dan mencatat perubahan ringkas di README GitHub.

## Desain antarmuka

Bagian atas menampilkan saldo utama, input cepat, dan konteks periode saat ini dalam urutan yang jelas. Filter transaksi dipadatkan pada layar kecil; daftar transaksi menggunakan jarak, kontras, dan tombol aksi yang mudah disentuh. Menu menyisakan aksi utama, sedangkan data pendukung tidak menutupi kontrol lain.

Dark mode tetap menjadi tampilan awal dan mode terang tetap tersedia. Semua permukaan input menggunakan token warna yang konsisten pada kedua tema.

## Interaksi dan aksesibilitas

Setiap panel/modal dapat dibuka dari keyboard, ditutup dengan Escape atau klik backdrop, menahan fokus selama terbuka, lalu mengembalikan fokus ke tombol pembuka. Feedback transaksi muncul dekat input dan status simpan tetap terlihat tanpa menggeser layout.

## Data dan kompatibilitas

Tidak ada perubahan pada nama key, bentuk akun/transaksi/anggaran/target/settings, atau format backup. Semua perubahan bersifat tampilan dan interaksi; alur simpan Supabase yang ada tetap dipakai.

## Verifikasi

- Uji statis untuk struktur modal, tombol, dan token tema.
- Pemeriksaan manual desktop dan lebar 375 px bila browser tersedia.
- Uji input transaksi, filter, buka/tutup modal, mode terang/gelap, serta ekspor/impor.
- Pastikan versi aplikasi dan README diperbarui.
