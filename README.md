# WangsitCoffee EDM

Email newsletter (HTML email) untuk WangsitCoffee, versi web di-host di Vercel.

- `index.html`: template email. Table-based, CSS inline, media query untuk mobile, fallback Outlook (MSO).
- Lebar 600px desktop, stack/fluid di bawah 600px.

## Preview lokal

Buka `index.html` di browser, atau:

```bash
yarn dlx serve .
```

## Deploy ke Vercel

```bash
yarn dlx vercel        # preview
yarn dlx vercel --prod # production
```

Framework preset: "Other". Tidak ada build step.

## Sebelum kirim

- Nama produk, harga, dan kode promo `WANGSIT15` masih contoh. Sesuaikan dengan data asli.
- Ganti link `#` (Lihat di browser, sosial media, preferensi, unsubscribe) dengan URL asli / merge tag ESP.
  Contoh Mailchimp: `*|ARCHIVE|*`, `*|UNSUB|*`.
- Gambar dari Unsplash (hotlink). Untuk produksi sebaiknya upload ke CDN sendiri.
- Tes di Litmus / Email on Acid atau kirim test ke Gmail, Outlook, Apple Mail.
