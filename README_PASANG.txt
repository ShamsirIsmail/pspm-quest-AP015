# PSPM QUEST V4.1 | PWA (AP015)

## Cara buka segera tanpa hosting
Buka fail `PSPM_QUEST_V4_1_Standalone.html` dalam browser. Ia boleh digunakan tanpa database dan tanpa internet. **Fail HTML setempat bukan pemasangan PWA penuh.**

## Cara jadikan app boleh dipasang
1. Upload **semua fail dalam folder ini** ke hosting HTTPS (contohnya GitHub Pages / Netlify / Cloudflare Pages), dengan `index.html` di root laman.
2. Pastikan `index.html`, `manifest.webmanifest`, `sw.js` dan folder `icons/` berada pada path yang sama seperti dalam ZIP.
3. Buka URL HTTPS pada telefon. Tekan `Cara pasang` di bahagian bawah home screen.
4. Android Chrome: Jika browser menyediakan install prompt, tekan `Install PSPM QUEST`. Jika tidak, buka menu browser > `Install app` / `Add to Home Screen`.
5. iPhone Safari: Buka halaman > Share > Add to Home Screen > Open as Web App > Add. Langkah perlu dibuat secara manual; website tidak boleh buka dialog Add to Home Screen iPhone secara automatik.
6. Buka aplikasi sekali semasa internet tersedia supaya service worker dapat menyimpan fail untuk penggunaan offline seterusnya.

## Database
Tidak perlu database untuk penggunaan peribadi/1 peranti. Semua 194 soalan kuiz, 66 Essay Builder dan progress tersimpan pada browser menggunakan localStorage. Tiada sync atau akaun pengguna. Kos hosting statik boleh sifar.

## Perhatian
- Soalan ialah latihan revision berdasarkan nota, bukan soalan rasmi/ramalan peperiksaan.
- Progress akan hilang jika data laman/browser dipadam. Progress PWA dan browser mungkin berbeza mengikut platform.
- Untuk update soalan, ganti fail dan ubah versi CACHE dalam `sw.js` untuk aktifkan fail baharu.

V4.1: Arahan Memory Flip boleh ditutup (tetapan disimpan pada peranti) dan feedback jawapan salah lebih mesra.
