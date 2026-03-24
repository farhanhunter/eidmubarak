# 🌙 Eid Mubarak 1447H — Static Landing Page

Halaman ucapan **Selamat Hari Raya Idul Fitri 1447 H** berbasis HTML statis murni. Tidak ada framework, tidak ada dependency — langsung buka di browser atau deploy ke static hosting manapun.

## ✨ Fitur

- **Countdown timer** — hitung mundur ke Idul Fitri 30 Mar 2026 00:00 WIB, auto-hide saat tercapai
- **Personal greeting** — tambahkan `?untuk=Nama` di URL, muncul "Kepada Nama," di atas teks Arab
- **Confetti burst** — 120 keping emas melayang saat halaman dibuka, auto-fade ~3 detik
- **Auto theme** — light mode pagi (jam 00–11), dark mode siang/malam (jam 12–23)
- **Toggle theme manual** — tombol ☀️/🌙 di pojok kanan atas untuk override auto-theme
- **Audio takbir** — autoplay muted, unmute otomatis saat interaksi pertama; tombol 🔊/🔇
- **Falling particles** — ◆ ✦ ◇ ✧ jatuh dari atas dengan rotasi, tampil di kedua tema
- **Share button** — Web Share API di mobile, fallback clipboard copy di desktop
- **Favicon inline SVG** — emoji 🌙, tanpa file eksternal
- **Social links** — LinkedIn & GitHub di footer
- Animasi bintang acak di langit malam (pure JS, dark mode only)
- Bulan sabit & bintang SVG dengan efek glow
- 3 lentera gantung animasi (swing effect)
- Teks Arab dengan font Amiri
- Kartu pesan dengan ornamen sudut emas
- Animasi masuk bertahap (staggered fade-in)
- SEO & Open Graph meta tags (WhatsApp, Twitter, dsb)
- Author credit — *developed by farhanhunter*
- Fully responsive — mobile friendly

## 🔗 Personal Greeting

Kirim link personal ke keluarga/teman dengan menambahkan query param `?untuk=`:

```
https://eidmubarak-gamma.vercel.app?untuk=Ibu
https://eidmubarak-gamma.vercel.app?untuk=Pak+Budi
https://eidmubarak-gamma.vercel.app?untuk=Tim+Engineering
```

Nama akan muncul otomatis: *"Kepada Ibu,"*

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
| Scripting  | Vanilla JS (stars, particles, countdown, confetti canvas, Web Share API) |
| Audio      | HTML5 `<audio>` — `takbir.mp3` (trimmed 5 min, 5.9MB) |
| Fonts      | Google Fonts — Amiri, Playfair Display, Cormorant Garamond (`display=optional`) |
| Assets     | Inline SVG + emoji favicon — zero external images |

## 📝 Last Update

| Versi | Tanggal       | Perubahan                                                                                                |
|-------|---------------|----------------------------------------------------------------------------------------------------------|
| 1.7.0 | 22 Maret 2026 | Countdown timer ke 25 Mar 2026 WIB; personal greeting `?untuk=Nama`; confetti burst 120 keping saat load |
| 1.6.0 | 22 Maret 2026 | Polish: `og:url`, light mode contrast, font `display=optional`, hapus unused CSS                         |
| 1.5.0 | 22 Maret 2026 | Favicon inline SVG emoji 🌙; social links LinkedIn & GitHub                                              |
| 1.4.0 | 22 Maret 2026 | CSS particle defaults di `:root`; author credit *developed by farhanhunter*; takbir.mp3                  |
| 1.3.0 | 22 Maret 2026 | Falling particles (◆✦◇✧); audio takbir + mute toggle                                                     |
| 1.2.0 | 22 Maret 2026 | Toggle theme manual; share button; SEO & Open Graph tags                                                 |
| 1.1.0 | 22 Maret 2026 | Auto light/dark theme; CSS `[data-theme]` refactor                                                       |
| 1.0.0 | 22 Maret 2026 | Initial release                                                                                          |

---

Made with ☾ for Idul Fitri 1447H — developed by farhanhunter