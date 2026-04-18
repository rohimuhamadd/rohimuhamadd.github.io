# Repository Guidelines

## Project Structure & Module Organization
Repository ini adalah static personal resume site berbasis HTML, CSS, dan vanilla JavaScript.
- `index.html`: entry point halaman utama dan struktur konten resume/portfolio.
- `css/styles.css`: styling utama (berasal dari Bootstrap theme yang sudah dimodifikasi).
- `js/scripts.js`: interaksi UI sederhana (scrollspy dan navbar behavior).
- `assets/img/`: semua image asset (profile photo, favicon, dll).
- `RESUME.md`: referensi konten resume dalam format Markdown.

Simpan perubahan sesuai domain file (konten di `index.html`, styling di `css/`, behavior di `js/`) untuk menjaga review tetap jelas.

## Build, Test, and Development Commands
Tidak ada build pipeline atau package manager di repo ini. Jalankan local preview dengan server sederhana:
- `python3 -m http.server 8000` untuk serve project di local.
- Buka `http://localhost:8000` untuk verifikasi tampilan.
- `git status` untuk cek file yang berubah sebelum commit.

Jika hanya update konten kecil, membuka `index.html` langsung di browser boleh, tapi tetap prefer local server agar relative path dan asset loading konsisten.

## Coding Style & Naming Conventions
- Gunakan indentasi 2 spasi di HTML/CSS, dan 4 spasi di JavaScript (ikuti style existing file).
- Pertahankan class naming yang deskriptif dan konsisten (`btn-portfolio`, `mb-mobile-15`, dst).
- Hindari inline style baru; prioritaskan penempatan style di `css/styles.css`.
- Jangan menambah framework baru tanpa kebutuhan jelas; project ini sengaja lightweight.

## Testing Guidelines
Testing dilakukan secara manual (belum ada automated test framework).
- Validasi section navigation (`About`, `Experience`, `Skills`, dst) berfungsi.
- Cek responsive layout minimal di mobile (<768px) dan desktop.
- Pastikan semua external link (LinkedIn, GitHub, portfolio, certificate) tidak broken.
- Verifikasi image utama di `assets/img/` tetap ter-load.

## Commit & Pull Request Guidelines
Dari history, format commit cenderung ringkas dan imperatif, misalnya `update resume` atau `add odoo certificate`.
- Gunakan pola: `<action> <scope singkat>` (contoh: `update resume links`, `fix mobile spacing`).
- Satu commit untuk satu tujuan perubahan.
- PR sebaiknya berisi:
  - ringkasan perubahan,
  - alasan perubahan,
  - screenshot sebelum/sesudah untuk perubahan UI,
  - checklist manual test yang sudah dijalankan.
