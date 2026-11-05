# Landing Page Kampanye Slamet

Landing page statis untuk **SLAMET — Calon Kepala Desa Tlagayasa, Periode 2027–2035**. Dibuat memakai HTML5, CSS3, dan JavaScript murni; siap dipublikasikan melalui GitHub Pages.

## Menjalankan

Buka `index.html` langsung di browser, atau gunakan ekstensi server lokal (misalnya Live Server) agar pengalaman pengujian lebih nyaman.

## Pengelolaan konten

- Seluruh data profil sementara, visi, tujuh misi, program, potensi, dan judul galeri berada di `js/data.js`. Ubah objek `profile` untuk memperbarui informasi calon tanpa menyentuh markup halaman.
- Foto kandidat tersimpan di `assets/images/slamet-profile.png`. Ganti file itu bila tersedia foto potret terpisah dengan nama yang sama.
- Delapan gambar placeholder lokal berada di `assets/images/gallery/`. Ganti berkas `gallery-01.jpg` hingga `gallery-08.jpg` dengan dokumentasi asli ketika tersedia; nama file dipertahankan agar galeri otomatis memperbarui tampilannya.
- Paket ikon kampanye berada di `assets/icons/color/` dan `assets/icons/monochrome/`. Ikon konten memakai varian berwarna; ikon aksi memakai varian monokrom agar mengikuti warna tombol melalui CSS.
- Placeholder profil sengaja dipertahankan pada bagian riwayat pendidikan, organisasi, pekerjaan, dan kegiatan kemasyarakatan karena data belum disediakan.

## Fitur

- Navigasi sticky responsif dan hamburger menu
- Panel visi expand/collapse
- Tujuh kartu misi interaktif dengan satu panel detail dinamis yang otomatis menjadi fokus layar
- Kartu program yang menautkan ke detail misi
- Galeri dengan lightbox, navigasi keyboard, dan tombol sebelumnya/berikutnya
- Animasi saat masuk viewport, indikator progres gulir, tombol kembali ke atas, serta dukungan `prefers-reduced-motion`

## Publikasi GitHub Pages

Unggah isi folder proyek ke repository GitHub. Pada **Settings → Pages**, pilih branch utama dan folder root (`/`). Setelah tersimpan, GitHub akan menampilkan alamat situs.
