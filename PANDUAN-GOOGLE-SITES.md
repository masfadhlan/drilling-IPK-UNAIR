# Cara memasang Bank Soal UAB IPK ke Google Sites

Isi folder ini adalah satu website statis:

- `index.html` berisi aplikasi beserta seluruh bank soal dan pembahasannya.
- `slides/` berisi 128 gambar slide PPT yang dipakai sebagai bukti di pembahasan.
- `qimg/` berisi gambar soal radiologi.

Ketiganya harus di-upload bersama dan struktur foldernya tidak boleh diubah.

Jangan paste `index.html` ke **Embed → Embed code** di Google Sites. Fitur itu menjalankan HTML di domain acak yang berganti setiap halaman dibuka. Akibatnya progres try-out, riwayat, dan daftar "Ulangi yang salah" hilang setiap refresh. Gambar slide juga tidak akan muncul.

## 1. Host di GitHub Pages (gratis)

1. Buat akun di github.com bila belum punya.
2. Klik **New repository**, beri nama misalnya `bank-soal-ipk`, pilih **Public**, lalu **Create repository**.
3. Klik **uploading an existing file**. Seret semua isi folder ini (`index.html`, folder `slides`, folder `qimg`, dan file lain) ke halaman upload, lalu klik **Commit changes**.
4. Buka **Settings → Pages**. Di bagian *Build and deployment*, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu **Save**.
5. Tunggu 1–2 menit. Alamat situs muncul di halaman yang sama, misalnya `https://namakamu.github.io/bank-soal-ipk/`. Buka alamat itu dan pastikan beranda serta gambar slide tampil.

## 2. Pasang di Google Sites

1. Di Google Sites, klik **Sisipkan → Sematkan (Embed)**, lalu pilih tab **Menurut URL (By URL)**.
2. Tempel alamat GitHub Pages dari langkah 1, pilih **Seluruh halaman (Whole page)**, lalu **Sisipkan**.
3. Tarik sudut kotak embed sampai cukup tinggi (minimal setinggi satu layar).
4. Tambahkan juga **Tombol (Button)** berlabel "Buka layar penuh" yang mengarah ke alamat yang sama. Tampilan di HP lebih nyaman lewat tab penuh, dan beberapa browser HP (terutama Safari di iPhone) membatasi penyimpanan data di dalam iframe.

## Catatan untuk teman-teman yang memakai

- Tidak perlu akun. Progres try-out, riwayat, dan daftar soal salah tersimpan di browser perangkat masing-masing.
- Data tersebut tidak ikut pindah ke perangkat lain dan akan hilang di mode incognito atau setelah data situs dihapus.
- Bila bank soal diperbarui, cukup upload ulang `index.html` (dan gambar baru bila ada) ke repository yang sama. Riwayat pengguna tetap aman.
