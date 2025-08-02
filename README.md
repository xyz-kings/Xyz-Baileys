
# <div align="center">WhatsApp Web API</div>

<div align="center">
  <img src="https://files.catbox.moe/2uswoi.png" alt="WhatsApp API" width="300"/>
</div>

---

Baileys adalah library TypeScript berbasis WebSocket untuk berinteraksi dengan **WhatsApp Web API**.  
Repository ini merupakan **versi modifikasi** dengan penambahan fitur untuk meningkatkan fleksibilitas dan memberikan pengalaman developer yang lebih baik.

> âš ï¸ **Catatan:** Ini bukan library resmi Baileys.

---

## ðŸ“Œ Table of Contents
- [Fitur](#-fitur)
- [Disclaimer](#-disclaimer)
- [Instalasi](#-instalasi)
- [Contoh Penggunaan](#-contoh-penggunaan)
- [Dokumentasi Lengkap](#-dokumentasi-lengkap)
- [Lisensi](#-lisensi)

---

## ðŸš€ Fitur
- Multi-Device Support (QR & Pairing Code)
- Manipulasi & Pengolahan Media (gambar, video, audio)
- System Events & Message Handling lengkap
- Group Management API
- Store & Session Management
- Utility Functions untuk WhatsApp Web API

---

## âš ï¸ Disclaimer
Proyek ini **tidak berafiliasi dengan, disetujui oleh, atau terhubung secara resmi dengan WhatsApp Inc., Meta Platforms, Inc., atau anak perusahaan mereka.**  
Situs resmi WhatsApp dapat ditemukan di [whatsapp.com](https://www.whatsapp.com).  
"WhatsApp", beserta nama, logo, dan merek terkait adalah milik intelektual dari pemiliknya masing-masing.

Versi modifikasi dari Baileys ini dibuat untuk membantu para developer, namun harus digunakan secara **bertanggung jawab**.  
Pengembang **sangat tidak menyarankan** penggunaan yang melanggar [Ketentuan Layanan WhatsApp](https://www.whatsapp.com/legal/terms-of-service).

> **Gunakan dengan risiko sendiri.** Hormati aturan platform, privasi, dan hukum yang berlaku.

---

## ðŸ“¥ Instalasi

### 1ï¸âƒ£ Install versi stable:
```bash
npm install github:ZVex-Dev/K-Baileys
```

### 2ï¸âƒ£ Install versi edge (fitur terbaru, tidak stabil):
```bash
yarn add github:ZVex-Dev/K-Baileys
```

### 3ï¸âƒ£ Import ke kode kamu:
```javascript
const { default: makeWASocket } = require("github:ZVex-Dev/K-Baileys");
```

---

## ðŸ› ï¸ Contoh Penggunaan
Coba jalankan contoh berikut:

1. Masuk ke direktori project:
   ```bash
   cd path/to/Baileys
   ```

2. Install dependensi:
   ```bash
   npm install
   ```

3. Jalankan contoh:
   ```bash
   node example.js
   ```

ðŸ‘‰ Lihat [example.ts](Example/example.ts) untuk implementasi lengkap.

---

## ðŸ“š Dokumentasi Lengkap
- [Docs Resmi Baileys](https://guide.whiskeysockets.io/)
- [WhatsApp Channel](https://whatsapp.com/channel/0029Vaj4X9iAInPuhzUk3v1L)

---

## ðŸ“„ Lisensi
Proyek ini dirilis di bawah lisensi **GPL-3.0** karena menggunakan [libsignal-node](https://git.questbook.io/backend/service-coderunner/-/merge_requests/1).
