# 👛 Doku · Dokat Ku

### Catat hari ini, lebih tenang esok hari.

**Doku** adalah aplikasi pencatatan keuangan pribadi untuk membantu mengenali ke mana uang pergi, memantau anggaran, dan membangun kebiasaan finansial yang lebih teratur.

Namanya berasal dari **“Dokat Ku”**, yang berarti **“Duit Ku”**. Kata *dokat* diambil dari sebutan uang dalam bahasa daerah yang digunakan pembuatnya di Tambun Selatan, Bekasi.

Dari ungkapan lokal yang akrab, menjadi ruang sederhana untuk merawat keuangan pribadi.

**[Buka aplikasi Doku →](https://ayyunnan.github.io/catatan-keuangan/index.html)**

## ✨ Apa yang bisa dilakukan?

- **Catat pemasukan dan pengeluaran** dengan tanggal, kategori, nominal, serta catatan tambahan.
- **Lihat ringkasan bulanan** untuk mengetahui pemasukan, pengeluaran, dan selisih transaksi.
- **Pantau anggaran mingguan** berdasarkan siklus dan tanggal yang dipilih.
- **Kenali tren keuangan** melalui grafik arus kas enam bulan dan komposisi pengeluaran.
- **Cari dan kelola transaksi** dengan pencarian, filter, serta fitur edit dan hapus.
- **Ekspor riwayat ke CSV** sesuai bulan dan filter yang sedang digunakan.
- **Akses dari ponsel atau laptop** melalui tampilan responsif.

> Selisih bulanan dihitung dari transaksi yang dicatat. Angka ini bukan saldo rekening bank dan tidak tersinkron otomatis dengan bank.

## 🎨 Sederhana dan nyaman digunakan

Doku menggunakan latar terang, aksen biru, dan ikon dompet sebagai identitas visual. Halaman masuk dan dashboard dibuat selaras, dengan navigasi yang memudahkan pencatatan sehari-hari.

Tujuannya sederhana: membuat mencatat keuangan terasa ringan dan mudah diulang.

## 🚀 Mulai menggunakan

1. Buka **[halaman Doku](https://ayyunnan.github.io/catatan-keuangan/index.html)**.
2. Buat akun menggunakan email pribadi.
3. Jika diminta, konfirmasi email melalui tautan yang dikirimkan.
4. Masuk, lalu tambahkan transaksi pertama.
5. Pilih bulan laporan untuk melihat ringkasan dan riwayat.

Gunakan fitur **Lupa kata sandi** pada halaman masuk jika membutuhkan pemulihan akses.

## 🧰 Teknologi

| Bagian | Teknologi |
|---|---|
| Antarmuka | HTML, CSS, dan JavaScript |
| Hosting situs | GitHub Pages |
| Autentikasi | Supabase Auth |
| Database | PostgreSQL melalui Supabase |
| Akses data | API Supabase |

GitHub Pages menyajikan halaman aplikasi. Supabase menangani autentikasi dan penyimpanan transaksi.

## 📂 Berkas utama

| Berkas | Kegunaan |
|---|---|
| `index.html` | Halaman masuk, pendaftaran, dan pemulihan kata sandi |
| `dashboard.html` | Ringkasan, transaksi, anggaran, tren, dan akun |
| `PANDUAN.md` | Panduan pendamping proyek |
| `supabase-setup.sql` | Berkas SQL untuk penyiapan Supabase |

## 🔐 Keamanan dan privasi

Dashboard memeriksa sesi sebelum menampilkan data. Pengguna tanpa sesi yang valid diarahkan ke halaman masuk.

**Perlindungan data tetap bergantung pada konfigurasi database.** Kebijakan *Row Level Security* atau RLS harus membatasi akses setiap pengguna ke transaksi miliknya sendiri.

Untuk pengelola proyek:

- Gunakan **publishable key** pada aplikasi browser.
- Jangan memasukkan **secret key**, **service role key**, atau kata sandi database ke repositori publik.
- Pastikan kebijakan baca, tambah, ubah, dan hapus transaksi memeriksa kepemilikan `user_id`.
- Sesuaikan alamat pengalihan autentikasi dengan alamat situs.
- Jangan mengunggah cadangan transaksi pribadi ke repositori publik.

Untuk pengguna, selalu keluar dari akun setelah menggunakan perangkat bersama.

## 💾 Cadangan dan pemeliharaan

Lakukan ekspor transaksi secara berkala dan simpan hasilnya di tempat yang aman.

**Ekspor CSV mengikuti bulan, pencarian, dan filter jenis transaksi yang aktif.** Satu ekspor tidak selalu mencakup seluruh riwayat. CSV transaksi juga bukan cadangan lengkap akun, skema database, atau konfigurasi keamanan.

Pengelola perlu memantau kapasitas database, penggunaan transfer data, dan status layanan Supabase secara berkala.

## 📝 Catatan penggunaan

- Doku merupakan alat pencatatan, bukan layanan perbankan atau dompet elektronik.
- Akurasi laporan bergantung pada kelengkapan transaksi yang dimasukkan.
- Nilai dan kategori anggaran bawaan dapat disesuaikan melalui kode.
- Nama kategori bersama tidak otomatis berarti data dibagikan kepada akun lain.
- Login dan sinkronisasi transaksi memerlukan koneksi internet.

## 🌱 Tentang proyek

Doku berangkat dari kebutuhan sehari-hari: mencatat uang masuk, memahami pengeluaran, dan menjaga anggaran agar lebih terarah.

Dikembangkan oleh **[ayyunnan](https://github.com/ayyunnan)**, dengan identitas lokal dari **Tambun Selatan, Bekasi**.

**Doku · Dokat ku, lebih teratur.**
