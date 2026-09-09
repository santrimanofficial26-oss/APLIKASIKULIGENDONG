# Vercel Deployment Wrapper — Kuli Gendong SDN 4 Rasau Jaya

Folder ini dirancang khusus untuk memendekkan (masking/wrapper) URL Google Apps Script Web App menjadi domain ringkas dan profesional di Vercel (misal: `kuligendong.vercel.app` atau domain kustom sekolah `literasi.sdn4rasaujaya.sch.id`).

---

## 🎯 Target URL Google Apps Script
```
https://script.google.com/macros/s/AKfycbyY_k6kWB1CJ1d7zqFpd1HVWNlAHltkj7szbgVxCgF7be7ZJx6q1FNhRJOw8VcdqTQWDQ/exec
```

---

## ✨ Fitur-Fitur Wrapper
1. **Full-Spectrum Meta SEO**:
   - Title, Meta Description, Keywords, Author, Robots, Geo-location (Rasau Jaya, Kubu Raya).
2. **Social Media Sharing (Open Graph & Twitter / X Card)**:
   - Tampilan card pratinjau yang indah saat dibagikan ke WhatsApp, Facebook, Telegram, dan Twitter/X.
3. **PWA & Mobile Ready**:
   - Theme-color `#012764` (Navy Brand).
   - Dynamic Viewport `100dvh` (mencegah overflow/potong akibat URL bar browser mobile).
   - Embedded SVG Favicon (tidak akan 404).
4. **Sleek Loading Screen (Shadcn Style)**:
   - Indikator progres halus dengan dual spinner dan logo halo yang otomatis memudar (*fade-out*) saat Web App selesai dimuat.
   - Tombol *fallback* otomatis jika koneksi pengguna lambat.
5. **Konfigurasi `vercel.json`**:
   - Header keamanan (`nosniff`, `XSS protection`, `Referrer-Policy`) dan optimasi `cleanUrls`.

---

## 🚀 Cara Deploy ke Vercel

### Metode A: Lewat Dashboard Vercel (Paling Mudah)
1. Buka [vercel.com](https://vercel.com) dan login dengan akun GitHub Anda.
2. Klik **Add New... > Project**.
3. Pilih repository **`santrimanofficial26-oss/APLIKASIKULIGENDONG`**.
4. Pada bagian **Root Directory**, klik **Edit** dan pilih folder **`vercel`**.
5. Klik tombol **Deploy**.
6. Selesai! Web app Anda langsung aktif di URL `https://[nama-project].vercel.app`.

### Metode B: Menggunakan Vercel CLI
```bash
cd vercel
npx vercel --prod
```
