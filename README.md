# Xyz-Baileys

Xyz-Baileys adalah bot WhatsApp berbasis Node.js yang menggunakan library `@whiskeysockets/baileys` versi modifikasi dari [ZVex-Dev/ZDev-Baileys](https://github.com/ZVex-Dev/ZDev-Baileys.git). Bot ini dirancang untuk memberikan pengalaman otomatisasi WhatsApp yang kaya fitur, mendukung Multi-Device, dan mudah disesuaikan untuk kebutuhan pengembang.

## Fitur Utama
- **Multi-Device Support**: Terhubung ke WhatsApp tanpa perlu scan QR berulang.
- **Pengolahan Media**: Mendukung gambar, video, audio, dan stiker dengan library seperti `fluent-ffmpeg` dan `jimp`.
- **Penerjemahan Teks**: Terjemahkan pesan ke berbagai bahasa menggunakan Google Translate API.
- **Pencarian dan Scraping**: Ambil data dari YouTube, Google Images, atau situs lain dengan `yt-search` dan `cheerio`.
- **Penjadwalan Tugas**: Otomatisasi tugas berbasis waktu dengan `node-cron`.
- **QR Code**: Buat dan baca QR code untuk interaksi dinamis.
- **Text-to-Speech**: Ubah teks menjadi suara dengan `node-gtts`.
- **Validasi Nomor**: Format dan validasi nomor telepon internasional dengan `awesome-phonenumber`.
- **Logging Efisien**: Gunakan `pino` untuk logging yang cepat dan ringan.

## Keunggulan
- **Ringan dan Cepat**: Dibangun dengan JavaScript dan Node.js untuk performa optimal.
- **Modular**: Struktur direktori (`src`, `lib`, `media`) memudahkan kustomisasi.
- **Lisensi MIT**: Bebas digunakan dan dimodifikasi dengan tanggung jawab penuh pada pengguna.
- **Komunitas Baileys**: Berbasis library populer dengan modifikasi untuk performa lebih baik.

## Instalasi
1. Clone repository ini:
   ```bash
   git clone https://github.com/xyz-kings/Xyz-Baileys.git
   cd Xyz-Baileys
   ```

2. Install dependensi:
    ```bash
   npm install
    ```
4. Jalankan bot:
    ```bash
   npm start
    ```


## Struktur Direktori
```bash
├── lib/              # Library dan utilitas
├── src/              # Source code bot
├── media/            # File media (gambar, video, dll.)
├── index.js          # Entry point
└── package.json      # Konfigurasi proyek
```

### Dependensi
####Berikut adalah dependensi utama yang digunakan:
   - @whiskeysockets/baileys: Library inti untuk WhatsApp Multi-Device.
   - fluent-ffmpeg: Pengolahan media (video/audio).
   - jimp: Manipulasi gambar.
   - node-gtts: Text-to-speech.
   - yt-search: Pencarian video YouTube.
   - node-cron: Penjadwalan tugas.
👉 Lihat package.json untuk daftar lengkap dibawah.

## Rekomendasi Tambahan

###Untuk meningkatkan fungsionalitas, pertimbangkan menambahkan:
   - @ffmpeg-installer/ffmpeg: Pastikan fluent-ffmpeg berjalan di semua sistem.
   - dotenv: Kelola variabel lingkungan dengan aman.
   - express: Tambahkan API endpoint untuk kontrol bot.
   - socket.io: Komunikasi real-time dengan aplikasi lain.


## Disclaimer

   - Proyek ini tidak berafiliasi, disetujui oleh, atau terhubung secara resmi dengan WhatsApp Inc., Meta Platforms, Inc., atau anak perusahaan mereka. Situs resmi WhatsApp dapat ditemukan di whatsapp.com. "WhatsApp", beserta nama, logo, dan merek terkait adalah milik intelektual dari pemiliknya masing-masing.

   - Versi modifikasi dari Baileys ini dibuat dengan tujuan membantu para developer, namun harus digunakan secara bertanggung jawab. Pengembang sangat tidak menyarankan penggunaan yang melanggar Ketentuan Layanan WhatsApp, termasuk tapi tidak terbatas pada:
       - spam,
       - pesan otomatis massal,
       - stalking,
       - scraping data pengguna,
       - atau penggunaan lain yang melanggar privasi, persetujuan, atau integritas platform.

   - Proyek ini disediakan apa adanya dan harus digunakan dengan sangat hati-hati. Kamu bertanggung jawab penuh atas bagaimana kamu menggunakan library ini. Pastikan penggunaannya etis, legal, dan menghormati hak serta privasi orang lain.

> ⚠️ Gunakan dengan risiko sendiri. Hormati aturan platform, batasan pengguna, dan tetap pada jalur hukum serta moral.




## Template package.json Baru

### Berikut adalah template package.json untuk repo baru Anda, berdasarkan package.json asli dengan beberapa penyesuaian dan tambahan rekomendasi:
```bash
{
  "name": "xyz-baileys",
  "version": "1.0.0",
  "description": "WhatsApp Bot Multi Device based on Baileys with enhanced features",
  "main": "index.js",
  "type": "commonjs",
  "directories": {
    "lib": "lib",
    "src": "src",
    "media": "media"
  },
  "scripts": {
    "start": "node index.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "xyz-kings",
  "license": "MIT",
  "repository": {
    "type": "git",
    "url": "https://github.com/xyz-kings/Xyz-Baileys.git"
  },
  "dependencies": {
    "@adiwajshing/keyed-db": "^0.2.4",
    "@hapi/boom": "^10.0.1",
    "@vitalets/google-translate-api": "^8.0.0",
    "@whiskeysockets/baileys": "github:xyz-kings/Xyz-Baileys",
    "awesome-phonenumber": "^5.9.0",
    "axios": "^1.4.0",
    "chalk": "^4.1.2",
    "cheerio": "^1.0.0-rc.12",
    "chokidar": "^4.0.3",
    "didyoumean": "^1.2.2",
    "file-type": "^16.5.3",
    "fluent-ffmpeg": "^2.1.2",
    "form-data": "^4.0.0",
    "fs-extra": "^11.1.1",
    "g-i-s": "^2.1.7",
    "got": "^11.8.3",
    "human-readable": "^0.2.1",
    "jimp": "^0.16.1",
    "jsdom": "^22.1.0",
    "lodash": "^4.17.21",
    "mal-scraper": "^2.13.2",
    "mathjs": "^11.3.0",
    "megajs": "^1.1.4",
    "moment-timezone": "^0.5.43",
    "ms": "^2.1.3",
    "node-cache": "^5.1.2",
    "node-cron": "^3.0.0",
    "node-fetch": "^2.6.1",
    "node-gtts": "^2.0.2",
    "node-os-utils": "^1.3.6",
    "node-webpmux": "^3.2.1",
    "parse-ms": "^2.1.0",
    "performance-now": "^2.1.0",
    "pino": "^8.14.1",
    "qrcode": "^1.5.3",
    "qrcode-reader": "^1.0.4",
    "qrcode-terminal": "^0.12.0",
    "similarity": "^1.2.1",
    "steno": "^1.0.0",
    "yt-search": "^2.10.4",
    "@ffmpeg-installer/ffmpeg": "^1.1.0",
    "dotenv": "^16.0.3",
    "express": "^4.18.2",
    "socket.io": "^4.5.4"
  }
}
```

## Penjelasan package.json
> Nama & Versi: xyz-baileys, versi awal 1.0.0.
Repository: https://github.com/xyz-kings/Xyz-Baileys.git.
Author: xyz-kings.
Dependencies: Semua dependensi asli dipertahankan + rekomendasi (@ffmpeg-installer/ffmpeg, dotenv, express, socket.io).
Scripts: Menambahkan test sebagai placeholder.

---

## Langkah Selanjutnya
   - 1. Clone repo baru Anda:
    ```bash
     git clone https://github.com/xyz-kings/Xyz-Baileys.git
     cd Xyz-Baileys
    ```
   - 2. Buat file README.md dan copy-paste isi dokumen ini.
   - 3. Buat file package.json dan copy-paste template di atas.
   - 4. Salin folder lib, src, media, dan file lain dari repo asli ZVex-Baileys ke repo baru.
   - 5. Jalankan:
     ```bash
     npm install
     ```
   - 6. Uji bot dengan:

npm start
