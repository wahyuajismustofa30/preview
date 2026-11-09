# Landing Page Kampanye Slamet

Landing page statis untuk **Slamet Purwanto (nama kampanye: SLAMET) — Calon Kepala Desa Tlagayasa, Periode 2027–2035**. Dibuat memakai HTML5, CSS3, dan JavaScript murni; siap dipublikasikan melalui GitHub Pages.

## Menjalankan

Buka `index.html` langsung di browser, atau gunakan ekstensi server lokal (misalnya Live Server) agar pengalaman pengujian lebih nyaman.

## Pengelolaan konten

- Data identitas calon, profil, visi, tujuh misi, program, potensi, dan judul galeri berada di `js/data.js`. Nama lengkap diatur melalui `candidate.fullName`; nama kampanye/brand tetap melalui `candidate.name`. Perbarui keduanya secara konsisten bila identitas publik berubah.
- Foto kandidat tersimpan di `assets/images/slamet-profile.png`. Ganti file itu bila tersedia foto potret terpisah dengan nama yang sama.
- Delapan gambar placeholder lokal berada di `assets/images/gallery/`. Ganti berkas `gallery-01.jpg` hingga `gallery-08.jpg` dengan dokumentasi asli ketika tersedia; nama file dipertahankan agar galeri otomatis memperbarui tampilannya.
- Paket ikon kampanye berada di `assets/icons/color/` dan `assets/icons/monochrome/`. Ikon konten memakai varian berwarna; ikon aksi memakai varian monokrom agar mengikuti warna tombol melalui CSS.
- Placeholder profil sengaja dipertahankan pada bagian riwayat pendidikan, organisasi, pekerjaan, dan kegiatan kemasyarakatan karena data belum disediakan.

## Dokumentasi proyek

- [Konteks proyek](docs/PROJECT_CONTEXT.md)
- [Panduan AI khusus proyek](docs/AI_GUIDELINES.md)
- [Arsitektur](docs/ARCHITECTURE.md)
- [Katalog aset](docs/ASSETS.md)
- [Testing dan verifikasi](docs/TESTING.md)
- [Keputusan teknis](docs/DECISIONS.md)
- [Changelog](docs/CHANGELOG.md)

## Fitur

- Navigasi sticky responsif dan hamburger menu
- Panel visi expand/collapse
- Tujuh kartu misi interaktif dengan satu panel detail dinamis yang otomatis menjadi fokus layar
- Kartu program yang menautkan ke detail misi
- Galeri dengan lightbox, navigasi keyboard, dan tombol sebelumnya/berikutnya
- Animasi saat masuk viewport, indikator progres gulir, satu tombol musik latar (Play/mute/unmute), serta dukungan `prefers-reduced-motion`

## Publikasi GitHub Pages

Unggah isi folder proyek ke repository GitHub. Pada **Settings → Pages**, pilih branch utama dan folder root (`/`). Setelah tersimpan, GitHub akan menampilkan alamat situs.

## Sinkronisasi Git

Skrip `SYNC - 26.11.03.sh` bekerja dari root repository dan hanya menambahkan
perubahan dari `projects/preview/` ke staging. Jika ada perubahan yang sudah
di-stage di luar folder tersebut, skrip berhenti agar tidak ikut ter-commit.
Skrip juga menolak push bila commit lokal yang belum terkirim mengubah file di
luar folder proyek.

Sebelum push, skrip menampilkan daftar commit yang akan dikirim dan meminta
konfirmasi. Sinkronisasi tetap ditujukan ke branch `main`; jalankan hanya
setelah memeriksa daftar commit dan memastikan push langsung ke branch tersebut
memang diinginkan.
