# Lumbung Duit: panduan memasang di HP

Isi paket ini:

- `index.html`: aplikasi Lumbung Duit
- `manifest.json`: nama, warna, dan ikon aplikasi untuk HP
- `sw.js`: membuat aplikasi tetap bisa dibuka tanpa internet
- `icons/`: ikon aplikasi berbagai ukuran

Semua file di atas harus diunggah bersama-sama, dengan susunan folder yang sama.

## 1. Unggah ke GitHub Pages (gratis)

1. Buat akun di github.com jika belum punya.
2. Ketuk tombol **New repository**. Beri nama `lumbung-duit`, pilih **Public**, lalu **Create repository**.
3. Pada halaman repository, pilih **uploading an existing file**.
4. Ekstrak file zip ini terlebih dahulu, lalu seret semua isinya (`index.html`, `manifest.json`, `sw.js`, `PANDUAN.md`, dan folder `icons`) ke halaman unggah. Ketuk **Commit changes**.
5. Buka **Settings → Pages**. Di bagian *Build and deployment*, pilih **Deploy from a branch**, branch **main**, folder **/ (root)**, lalu **Save**.
6. Tunggu 1–2 menit. Alamat aplikasi Anda akan tampil di halaman itu, misalnya `https://namaanda.github.io/lumbung-duit/`.

Catatan: unggah lewat laptop jauh lebih mudah daripada lewat HP.

## 2. Pasang di HP Android

1. Buka alamat tadi di **Chrome**.
2. Ketuk menu **⋮**, lalu pilih **Instal aplikasi** (atau **Tambahkan ke layar utama**).
3. Ikon Lumbung Duit akan muncul di layar depan HP. Aplikasi terbuka layar penuh dan tetap bisa dipakai tanpa internet.

## 3. Pindahkan data dari versi lama (claude.ai)

Data tidak pindah otomatis karena alamatnya berbeda.

1. Di versi lama, buka **Atur → Simpan cadangan (JSON)**.
2. Di versi baru, buka **Atur → Pulihkan cadangan**, lalu pilih file cadangan tadi.

## Penting tentang data

- Data keuangan Anda **hanya tersimpan di HP Anda**, tidak pernah diunggah ke GitHub. Yang publik hanya kode aplikasinya.
- Menghapus data Chrome atau mencopot aplikasi akan menghapus catatan Anda. Rutin **Simpan cadangan (JSON)**, misalnya seminggu sekali, dan simpan file-nya di Google Drive.
- Setiap orang yang membuka alamat yang sama memiliki data masing-masing di HP-nya sendiri.

## Memperbarui aplikasi

1. Ganti file yang berubah di GitHub (unggah ulang dengan nama yang sama).
2. Buka `sw.js` dan naikkan nomor versinya, misalnya dari `lumbung-duit-v1` menjadi `lumbung-duit-v2`.
3. Buka aplikasi di HP saat ada internet. Tutup lalu buka sekali lagi, dan versi baru akan aktif.
