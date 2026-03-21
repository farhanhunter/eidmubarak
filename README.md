# 🌙 Eid Mubarak 1447H — Static Landing Page

Halaman ucapan **Selamat Hari Raya Idul Fitri 1447 H** berbasis HTML statis murni. Tidak ada framework, tidak ada dependency — langsung buka di browser atau deploy ke static hosting manapun.

## ✨ Fitur

- **Auto theme** — light mode pagi (jam 00–11), dark mode siang/malam (jam 12–23)
- **Toggle theme manual** — tombol ☀️/🌙 di pojok kanan atas untuk override auto-theme
- **Audio takbir** — autoplay muted, unmute otomatis saat interaksi pertama; tombol 🔊/🔇
- **Falling particles** — ◆ ✦ ◇ ✧ jatuh dari atas dengan rotasi, tampil di kedua tema
- **Share button** — Web Share API di mobile, fallback clipboard copy di desktop
- **Favicon inline SVG** — emoji 🌙, tanpa file eksternal
- Animasi bintang acak di langit malam (pure JS, dark mode only)
- Bulan sabit & bintang SVG dengan efek glow
- 3 lentera gantung animasi (swing effect)
- Teks Arab dengan font Amiri
- Kartu pesan dengan ornamen sudut emas
- Animasi masuk bertahap (staggered fade-in)
- SEO & Open Graph meta tags (WhatsApp, Twitter, dsb)
- Author credit — *developed by farhanhunter*
- Fully responsive — mobile friendly

## 🗂️ Struktur

```
eidmubarak/
├── index.html      # Seluruh halaman (HTML + CSS + JS inline)
├── takbir.mp3      # Audio takbir (trimmed 5 min, 5.9MB)
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
| Styling    | CSS3 (custom properties, keyframes, `[data-theme]`) |
| Scripting  | Vanilla JS (star field, auto theme, Web Share API, particles) |
| Audio      | HTML5 `<audio>` — `takbir.mp3` (trimmed 5 min, 5.9MB) |
| Fonts      | Google Fonts — Amiri, Playfair Display, Cormorant Garamond |
| Assets     | Inline SVG + emoji favicon — zero external images |

## 📝 Last Update

| Versi | Tanggal       | Perubahan                                      |
|-------|---------------|------------------------------------------------|
| 1.5.0 | 22 Maret 2026 | Favicon inline SVG emoji 🌙 — fix 404 favicon.ico |
| 1.4.0 | 22 Maret 2026 | CSS particle defaults di `:root`; author credit *developed by farhanhunter*; takbir.mp3 di-commit ke repo |
| 1.3.0 | 22 Maret 2026 | Falling particles (◆✦◇✧) dengan negative delay; audio takbir + tombol mute; autoplay muted strategy |
| 1.2.0 | 22 Maret 2026 | Toggle theme manual (☀️/🌙); share button (Web Share API + clipboard fallback); SEO meta description; Open Graph tags |
| 1.1.0 | 22 Maret 2026 | Auto light/dark theme berdasarkan jam lokal; stars hidden di light mode; CSS refactor ke `[data-theme]` variables |
| 1.0.0 | 22 Maret 2026 | Initial release — Idul Fitri 1447H landing page |

---

Made with ☾ for Idul Fitri 1447H — developed by farhanhunter