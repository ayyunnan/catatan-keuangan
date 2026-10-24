# Catatan Keuangan — publikasi gratis

Aplikasi menggunakan GitHub Pages untuk situs dan Supabase untuk database cloud. GitHub Pages saja tidak menyimpan transaksi antarperangkat.

## Database
1. Buat proyek di https://supabase.com/.
2. Buka SQL Editor, jalankan seluruh isi `supabase-setup.sql`.
3. Buka Project Settings/API, salin Project URL dan publishable key (atau anon key lama). Jangan gunakan service_role/secret key.
4. Pastikan metode Email aktif pada Authentication.

## Hosting GitHub Pages
1. Masuk ke https://github.com/ dan buat repository `catatan-keuangan`.
2. Upload `index.html`, `supabase-setup.sql`, dan `PANDUAN.md` ke root repository.
3. Buka Settings > Pages, pilih Deploy from a branch, branch `main`, folder `/(root)`, lalu Save.
4. URL umumnya `https://USERNAME.github.io/catatan-keuangan/`.

## Penggunaan lintas perangkat
Buka URL, isi URL dan publishable/anon key, klik Hubungkan, lalu daftar/masuk. Di perangkat lain gunakan URL/key yang sama dan masuk dengan akun yang sama.

Fitur: transaksi pemasukan/pengeluaran, rekap per bulan, kategori, hapus transaksi, ekspor CSV. Kebijakan Row Level Security membatasi transaksi ke akun pemiliknya. Simpan cadangan CSV berkala.
