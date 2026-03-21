# 🌙 Eid Mubarak 1447H — Static Landing Page

Halaman ucapan **Selamat Hari Raya Idul Fitri 1447 H** berbasis HTML statis murni. Tidak ada framework, tidak ada dependency — langsung buka di browser atau deploy ke static hosting manapun.

## ✨ Fitur

- Animasi bintang acak di langit malam (pure JS)
- Bulan sabit & bintang SVG dengan efek glow
- 3 lentera gantung animasi (swing effect)
- Teks Arab dengan font Amiri
- Kartu pesan dengan ornamen sudut emas
- Animasi masuk bertahap (staggered fade-in)
- Fully responsive — mobile friendly

## 🗂️ Struktur

```
eidmubarak/
├── index.html      # Seluruh halaman (HTML + CSS + JS inline)
├── .gitignore
└── README.md
```

## 🚀 Deploy

### Vercel
```bash
vercel --prod
```

### GitHub Pages
Aktifkan di **Settings → Pages → Branch: main → / (root)**

### Manual
Cukup buka `index.html` di browser — tidak perlu server.

## 🛠️ Tech Stack

| Layer      | Detail                          |
|------------|---------------------------------|
| Markup     | HTML5                           |
| Styling    | CSS3 (custom properties, keyframes) |
| Scripting  | Vanilla JS (star field generator) |
| Fonts      | Google Fonts — Amiri, Playfair Display, Cormorant Garamond |
| Assets     | Inline SVG — zero external images |

## 📝 Last Update

| Versi | Tanggal        | Perubahan                                      |
|-------|----------------|------------------------------------------------|
| 1.0.0 | 22 Maret 2026  | Initial release — Idul Fitri 1447H landing page |

---

Made with ☾ for Idul Fitri 1447H
