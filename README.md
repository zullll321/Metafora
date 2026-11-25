# METAFORA — Website Media & Studio Kreatif

Website satu halaman (single-file) untuk **METAFORA — Media Pustaka Informasi**, media dan studio kreatif yang melayani publikasi, dokumentasi foto & video, siaran langsung, serta pembuatan website dan aplikasi.

- **File utama:** `index.html` (±1,78 MB, semua gambar sudah tertanam di dalam file)
- **Versi patokan:** 24 November 2026 — patokan `anjay.html` + logo menu ukuran B + perbaikan bug 1–5
- **Tanpa build tool:** cukup HTML, CSS, dan JavaScript biasa. Tidak perlu `npm install`.

---

## 1. Cara membuka

1. Simpan `index.html` di satu folder (mis. `E:\WEB METAFORA\`).
2. Klik dua kali file tersebut, buka dengan **Chrome** atau **Edge**.
3. Perangkat perlu internet hanya untuk font (Inter Tight dari Google Fonts) dan link keluar. Tanpa internet, halaman tetap tampil dengan font sistem.

> **Penting — preview vs browser.** Preview di aplikasi (panel samping, pratinjau file di HP) memakai lebar sempit dan sering membatasi JavaScript, sehingga tampilan bisa berbeda: animasi tidak jalan, carousel diam, halaman detail tidak terbuka. Nilailah tampilan dari file yang **dibuka di browser**. Sejak perbaikan no. 4, portofolio, proses, fitur, dan teks berjalan tetap tampil walau JavaScript mati.

---

## 2. Struktur halaman

| Urutan | Bagian | ID / alamat | Isi |
|---|---|---|---|
| 1 | Menu atas | — | Logo METAFORA, Layanan, Tentang, Portofolio, Berita, Kerja Sama, tombol "Hubungi kami" |
| 2 | Hero | `#hero` | Judul, deskripsi, objek 3D yang bergerak mengikuti kursor/scroll |
| 3 | Teks berjalan | — | Daftar layanan |
| 4 | Layanan | `#layanan` | 4 kartu berilustrasi: Media & Publikasi, Dokumentasi, Siaran Langsung, Solusi Digital |
| 5 | Ragam karya | `#media` | Carousel 3D (geser / panah / keyboard) |
| 6 | Tentang | `#tentang` | Maskot + 2 kartu (Media & kreatif, Solusi digital) |
| 7 | Fitur | `#fitur` | 8 kartu nilai kerja |
| 8 | Proses | `#proses` | 6 langkah, animasi scroll bertahap |
| 9 | Portofolio | `#portofolio` | Kartu portofolio + tombol "Lihat semua portofolio" |
| 9b | Berita terbaru | `#berita-terbaru` | Dinding 3D bergulir berisi 12 berita terbaru; tersembunyi bila berita tampil < 3 |
| 10 | Kerja Sama | `#paket` | Iklan & jasa, tombol WA "Tanya iklan" / "Konsultasi jasa" |
| 11 | FAQ | `#faq` | 4 pertanyaan, animasi scroll bertahap |
| 12 | Kontak + footer | `#kontak` | WA, Instagram, TikTok, alamat kantor, tautan halaman, tombol tema |
| — | Tombol WA melayang | — | Pojok kanan bawah, ke WA utama |

**Halaman portofolio (tanpa pindah file):**
- `index.html#/portofolio` — semua portofolio + filter kategori
- `index.html#/portofolio/<id-proyek>` — detail proyek (deskripsi, latar belakang, ruang lingkup, dokumentasi visual yang bisa diperbesar)

**Halaman berita (tanpa pindah file):**
- `index.html#/berita` — daftar berita, urut dari tanggal terbaru, dengan filter kategori (Semua, Kabar METAFORA, Lokal, Nasional, Teknologi, Pendidikan, Ekonomi Kreatif; kategori tanpa berita tidak ditampilkan). Isi `kategori` berita dengan salah satu nama itu persis. Selama data kosong tampil "Berita segera hadir" + tombol Instagram @_metaforaid
- `index.html#/berita/<id-berita>` — detail berita (kategori, tanggal, judul, ringkasan, foto yang bisa diperbesar, isi, sumber opsional)

---

## 3. Portofolio

| No | ID | Proyek | Tautan |
|---|---|---|---|
| 01 | `media-pcm-gombong` | Pengelolaan Media dan Publikasi PCM Gombong | — (belum ada tombol "Kunjungi website") |
| 02 | `website-pcm-gombong` | Pengembangan dan Pengelolaan Website Resmi PCM Gombong | https://pcmgombong.or.id |
| 03 | `website-pkbh-unimugo` | Pengembangan Website PKBH Universitas Muhammadiyah Gombong | https://pkbhunimugo.vercel.app/ |
| 04 | `website-payd-gombong` | Pengembangan Website MCC/LKSA PAYD Muhammadiyah Gombong | https://paydmgombong.vercel.app |
| 05 | `academic-hub-ai-task-manager` | Academic Hub — AI Task Manager (akses terbatas, perlu akun) | https://ai-task-manager-nextjs.vercel.app/ |

Ketentuan konten portofolio:
- Narasi 01–03 dari materi resmi user; narasi 04–05 disusun dari isi website dan penjelasan user — **perlu dicek ulang oleh tim**.
- Tidak ada proyek fiktif, testimoni, atau angka capaian yang tidak diberikan.
- Gambar adalah tangkapan layar asli (diambil 24 November 2026). Data akun pada screenshot Academic Hub sudah disamarkan.
- Kategori filter (Media Management, Photography & Videography, Website Development, Information Systems, Design & Branding, Digital Solutions) adalah struktur pengelompokan, bukan klaim semua kategori sudah punya proyek.

---

## 4. Kontak yang terpasang

| Kanal | Nilai |
|---|---|
| WhatsApp utama (tombol melayang, "Hubungi kami", tombol Kerja Sama) | Evan Dwi Andriano — 0812-3130-2394 (`wa.me/6281231302394`) |
| WhatsApp kedua | Zulfikar Ilmi Santoso — +62 813-8313-8011 (`wa.me/6281383138011`) |
| Instagram | https://www.instagram.com/_metaforaid/ |
| TikTok | https://www.tiktok.com/@_metaforaid |
| Alamat kantor | Gedung Dakwah Muhammadiyah Gombong — https://share.google/KKpYotQrsNemMm5R0 |

Setiap tombol WA membuka chat dengan pesan pembuka otomatis.

---

## 5. Cara mengubah isi

Semua isi berada di dalam `index.html`. Buka dengan editor teks (VS Code / Notepad++), lalu cari bagian berikut:

| Yang diubah | Cari di file | Catatan |
|---|---|---|
| Judul, paragraf, label | teks langsung di HTML (atribut `data-b="t.kNN"`) | Ubah teksnya saja, jangan hapus atributnya |
| Teks berjalan, fitur, langkah proses, carousel | `<script type="application/json" id="content">` | Kunci `mq`, `f`, `s`, `g` |
| Data portofolio | `<script type="application/json" id="pfdata">` | Satu objek per proyek: `n` nama, `cat` kategori, `tags` filter, `client`, `url`, `short`, `desc`, `bg`, `scope`, `value`, `cover`, `docs` |
| Gambar portofolio | `<script type="application/json" id="pfimg">` | Gambar dalam format base64 (data URI) |
| Berita | `<script type="application/json" id="brdata">` | Array objek: `id`, `judul`, `tanggal` (YYYY-MM-DD), `kategori`, `ringkas`, `isi` (array paragraf), `foto` (kunci di `brimg`), `keterangan_foto`, `sumber` (opsional). Contoh format ada di komentar tepat di atasnya |
| Foto berita | `<script type="application/json" id="brimg">` | `"kunci": "data:image/jpeg;base64,..."` |
| Warna | `:root{ --bg … --pri … }` di awal `<style>` | Ada versi terang dan gelap |

Peringatan:
- Simpan cadangan sebelum mengedit. Satu tanda kutip atau koma yang hilang di blok JSON membuat bagian itu tidak tampil.
- Isi cadangan tanpa JavaScript (di dalam `#pfgrid`, `#steps`, `#feat`, `#mq`) adalah salinan statis. Jika data di JSON diubah, salinan statis ini tidak ikut berubah — hanya terlihat saat JavaScript mati. Minta regenerasi bila perlu.

---

## 6. Online-kan (deploy)

File ini masih lokal. Agar bisa dibuka orang lain lewat alamat web, pilih salah satu (semuanya punya paket gratis):

1. **Vercel / Netlify** — buat project baru, unggah folder berisi `index.html`. Hasil: alamat seperti `metafora-xxx.vercel.app`, bisa disambungkan ke domain sendiri.
2. **GitHub Pages** — unggah `index.html` ke repository, aktifkan Pages.
3. **Hosting / cPanel** — unggah `index.html` ke folder `public_html`.

Setelah online, uji ulang di HP dan laptop.

---

## 7. Dukungan perangkat (sudah diuji)

| Perangkat | Lebar | Menu |
|---|---|---|
| HP / tablet kecil | 375–759 px | Tombol ☰ |
| Tablet / HP landscape | 760–1023 px | Menu lengkap |
| Laptop / desktop | ≥ 1024 px | Menu lengkap |

- Animasi Proses & FAQ aktif di desktop, laptop pendek (1366×768, 1280×600), tablet, dan HP; otomatis menjadi daftar biasa jika layar terlalu pendek.
- Mode terang/gelap mengikuti sistem, bisa diganti dari footer.
- Menghormati pengaturan "kurangi gerak" (reduced motion).
- Tidak ada error di console, tidak ada ID ganda, tidak ada link internal patah, tidak ada halaman melebar ke samping (uji 7 ukuran layar).

---

## 8. Catatan yang perlu diketahui

- **Maskot** di bagian Tentang memakai gambar karakter milik pihak lain. Risiko hak cipta sudah disampaikan dan diterima tim. Untuk jangka panjang disarankan maskot orisinal METAFORA.
- **Portofolio 01** belum punya tombol "Kunjungi website" di patokan ini.
- **Berita** saat ini berisi 12 berita pilihan dari media lain (dicek 25 Nov 2026). Hanya judul, ringkasan satu kalimat tulisan sendiri, dan tautan ke sumber — **jangan menyalin isi atau foto berita media lain**. Perbarui berkala; ganti dengan berita METAFORA sendiri bila sudah ada (slot `berita-01`…`berita-12`).
- **Academic Hub** bersifat akses terbatas; pengunjung hanya akan melihat halaman login.
- Target sentuh tombol menu (±38 px) dan baris FAQ mode ringkas (±28–32 px) sedikit di bawah ukuran ideal 44 px; sengaja dipertahankan agar animasi tetap muat di layar pendek.

---

## 9. Riwayat perubahan

| Tanggal | Perubahan |
|---|---|
| 24 Nov 2026 | Patokan ditetapkan dari `anjay.html` (logo asli, warna biru-cyan, kontak & WA, maskot, 5 portofolio, 4 layanan) |
| 24 Nov 2026 | Logo menu atas diperkecil (20 px desktop / 17 px HP); logo footer tetap |
| 24 Nov 2026 | Perbaikan: menu ☰ miring (HP/tablet), menu lengkap di tablet (kini ≥760 px), animasi Proses/FAQ di laptop pendek, isi tetap tampil tanpa JavaScript, tombol Back kembali ke posisi terakhir |
| 25 Nov 2026 | Portofolio 02 Web PCM: tambah 1 gambar dokumentasi (halaman Berita dengan pilihan bahasa) |
| 25 Nov 2026 | Menu & halaman Berita (`#/berita`, `#/berita/<id>`); isi berita menunggu data asli dari tim |
| 25 Nov 2026 | Teks layanan Solusi Digital diperbarui (website & toko online, sistem informasi & dashboard, kasir POS & stok, presensi digital & otomasi AI/Telegram/WA); disamakan di Kerja Sama, teks berjalan, carousel |
| 25 Nov 2026 | Bagian "Berita terbaru" di beranda (dinding 3D bergulir, 12 berita terbaru, muncul otomatis bila ≥ 3 berita tampil) + 12 slot berita siap isi di `brdata` |
| 25 Nov 2026 | 12 berita pilihan dari media lain (lokal Kebumen, nasional, teknologi, pendidikan, ekonomi kreatif) — judul, ringkasan sendiri, tautan ke sumber asli |
| 25 Nov 2026 | Filter kategori di halaman Berita (Semua, Kabar METAFORA, Lokal, Nasional, Teknologi, Pendidikan, Ekonomi Kreatif); kategori kosong disembunyikan |
| 25 Nov 2026 | Perbaikan HP: tidak lagi terlempar ke FAQ saat bar alamat browser muncul/hilang; posisi baca tetap saat layar diputar; dinding berita lebih rapi di tablet & HP |

---

## 10. Aturan kerja untuk revisi berikutnya

Setiap permintaan edit diajukan dulu dengan: **letak** (opsi posisi), **dampak** di desktop/tablet/HP, **risiko** bila dipaksakan, dan **rekomendasi**. Dikerjakan setelah disetujui. Bagian di luar permintaan tidak diubah. Setelah selesai, diuji di HP, tablet, laptop, dan desktop.
