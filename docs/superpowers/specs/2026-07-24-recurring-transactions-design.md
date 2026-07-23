# Transaksi Berulang IOT

IOT akan menyimpan aturan transaksi berulang—nama, nominal, jenis, kategori, akun, tanggal jatuh tempo, dan interval bulanan—secara terpisah dari riwayat transaksi. Saat aplikasi dibuka, aturan yang jatuh tempo akan tampil sebagai pengingat. Pengguna harus menekan tombol catat sebelum transaksi dibuat, sehingga tidak ada transaksi otomatis atau duplikat tanpa persetujuan.

Aturan disimpan di key Supabase baru `recurring_rules`; data akun dan transaksi lama tidak diubah. Antarmuka diletakkan di Menu sebagai modal sederhana untuk menambah, melihat, dan menghapus aturan. Setelah dicatat, tanggal jatuh tempo aturan maju satu interval bulan.
