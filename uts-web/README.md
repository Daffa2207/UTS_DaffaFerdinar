# My Profile - UTS Pemrograman Web 1

Website statis (HTML + CSS + sedikit JavaScript), tanpa framework dan tanpa proses build.

## Struktur folder

```
index.html            Beranda (gambar, video, musik latar)
daftar.html           Halaman bullet numbering
tabel.html            Halaman tabel
frame.html            Halaman frame (frameset)
  frame-menu.html     Isi frame kiri
  frame-isi.html      Isi frame kanan (default)
  frame-keahlian.html
  frame-pendidikan.html
iframe.html           Halaman iframe
  iframe-isi.html     Halaman yang ditampilkan di dalam iframe
css/style.css         Satu-satunya file CSS (warna ada di :root bagian atas)
img/                  Gambar (ganti foto-profil.jpg dengan foto lain jika perlu)
media/                video-profil.mp4 dan musik-latar.mp3
```

## Mengedit di Visual Studio Code

1. Buka VS Code, pilih **File > Open Folder**, lalu pilih folder ini.
2. Install ekstensi **Live Server** (VS Code akan menyarankannya otomatis).
3. Klik kanan `index.html`, pilih **Open with Live Server**. Setiap simpan file, browser ikut refresh.

Bagian yang paling sering diubah:
- Teks profil: `index.html`, `daftar.html`, `tabel.html`
- Warna: variabel `--navy`, `--teal`, `--sky`, `--mint` di bagian atas `css/style.css`
- Foto, video, musik: ganti file di `img/` dan `media/` dengan nama yang sama

## Hosting gratis

Pastikan seluruh isi folder diupload dengan struktur yang sama dan `index.html` ada di paling atas.

**Netlify (paling mudah)**
1. Buka app.netlify.com/drop.
2. Seret seluruh folder ini ke halaman tersebut.
3. Link website langsung jadi.

**GitHub Pages**
1. Buat repository baru di GitHub, lalu upload semua isi folder ini.
2. Buka **Settings > Pages**, pilih branch `main` dan folder `/ (root)`, lalu **Save**.
3. Link muncul dalam beberapa menit: `https://USERNAME.github.io/NAMA-REPO/`

**Hosting lain (InfinityFree, Hostinger, dll.)**
Upload semua isi folder ke folder `htdocs` atau `public_html` lewat File Manager atau FTP.

## Catatan

- Musik latar baru berbunyi setelah pengunjung menyentuh atau mengklik halaman (aturan browser).
- Peta di `iframe.html` butuh koneksi internet.
- `frame.html` memakai `<frameset>` karena diminta soal. Tag ini sudah usang di HTML5, tetapi masih berjalan di semua browser utama.
