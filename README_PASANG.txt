# PSPM QUEST V5.1 | PWA (AP015)

Aplikasi mudah alih ulang kaji Pengajian Perniagaan AP015 Matrikulasi Malaysia.
Mengandungi 194 soalan latih tubi, 66 latihan rangka esei, kad ingatan dan formula pengiraan.

## Cara Buka Segera (Luar Talian / Setempat)
Buka fail `index.html` menggunakan pelayar web (Google Chrome / Safari / Edge). Aplikasi boleh terus digunakan tanpa pangkalan data dan tanpa internet.

## Cara Jadikan Aplikasi Boleh Dipasang (PWA)
1. Muat naik semua fail dalam folder ini ke perkhidmatan hosting HTTPS (contohnya GitHub Pages, Netlify, atau Cloudflare Pages), dengan `index.html` berada pada direktori utama (root).
2. Pastikan `index.html`, `manifest.webmanifest`, `sw.js` dan folder `icons/` berada pada susunan direktori yang sama.
3. Buka URL HTTPS pada telefon pintar anda. Tekan butang `Panduan Pasang ↗` pada halaman utama aplikasi.
4. **Android (Chrome)**: Jika pelayar memaparkan dialog pemasangan, tekan `Pasang PSPM QUEST`. Jika tidak, tekan menu tiga titik (⋮) pelayar > pilih `Pasang aplikasi (Install app)` atau `Tambah ke Skrin Utama`.
5. **iPhone (Safari)**: Buka pautan dalam Safari > tekan ikon `Kongsi (Share)` > pilih `Tambah ke Skrin Utama (Add to Home Screen)` > tekan `Tambah (Add)`.
6. Buka aplikasi sekali semasa sambungan internet tersedia supaya Service Worker dapat menyimpan fail cache untuk kegunaan luar talian sepenuhnya.

## Pangkalan Data & Storan
Tiada pelayan atau pangkalan data luar diperlukan. Semua 194 soalan kuiz, 66 cabaran esei, dan kemajuan rekod pembelajaran disimpan secara setempat dalam pelayar menggunakan `localStorage`. Tiada akaun pengguna diperlukan dan kos pengehosan statik adalah percuma.

## Pembaharuan Versi 5.1 (V5.1 - Final QA & Deployment Release)
- Pengesahan Kandungan Akademik: 194 soalan kuiz (146 teori + 48 formula pengiraan) dan 66 cabaran esei disahkan 100% bebas ralat matematik, duplikasi atau pilihan jawapan kosong.
- Ketahanan PWA & Subdirektori: Diuji dan disahkan serasi sepenuhnya dengan GitHub Pages (`/pspm-quest-AP015/`).
- Pengemaskinian Cache Pintar: Service Worker `pspm-quest-v5.1-offline-1` dengan strategi Network-First untuk navigasi memastikan pengguna V4.1 sedia ada menerima kandungan terkini secara automatik tanpa perlu buang aplikasi atau hilang rekod kemajuan.
- Responsif Menyeluruh: Diuji pada resolusi 320px, 375px, 390px, 430px dan paparan desktop tanpa sebarang limpahan mendatar (horizontal overflow).
