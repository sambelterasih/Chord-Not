# ChordSasy — Mobile Web App

## Jalankan di HP
- Ekstrak ZIP dan buka `index.html` di Chrome.
- Untuk pemasangan sebagai PWA dan penggunaan offline, unggah seluruh isi folder ke hosting HTTPS statis (misalnya Cloudflare Pages). Buka URL-nya di Chrome Android → menu ⋮ → Tambahkan ke layar utama / Install app.
- File lokal `file://` tetap dapat membuka editor, tetapi service worker/PWA membutuhkan HTTPS atau localhost.

## Fitur
- Antarmuka mobile-first dengan navigasi bawah dan editor chord berbentuk bottom sheet.
- Mode Angka, Simple, Chord; transposisi; pilihan birama.
- Tambah bagian, tambah birama, edit ketukan, Undo/Redo.
- Pustaka lagu, pencarian, autosave lokal.
- Impor teks/TXT, impor PDF berbasis teks (PDF.js dimuat dari CDN saat diperlukan), backup/restore JSON.
- Ekspor TXT, backup lengkap, cetak/simpan PDF melalui dialog print.
- Tema terang/gelap, manifest dan service worker.

## Batasan yang diketahui
- Penyimpanan lokal per browser/perangkat; tidak ada sinkronisasi cloud.
- PDF hasil scan membutuhkan OCR dan belum didukung.
- PDF import mengeluarkan teks mentah; format perlu diperiksa sebelum diimpor.
- 6/8, 7/8, 12/8 ditampilkan sebagai 6, 7, 12 slot ketukan/subdivisi. Penafsiran ritmis compound meter tidak otomatis.
- Tidak ada AI chord recognition/audio analysis di versi ini.
