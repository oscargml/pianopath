# 🎹 PianoPath

> **Learn piano the fun way — play, don't just practice.**
> A free, interactive online piano with light-up chords & scales, play-along songs, ear-training games, and 16 step-by-step lessons. No download, no sign-up, 100% in the browser.

**Live:** https://pianopath.vercel.app/

---

## ✨ Features

- **Interactive piano** — real-time sound via the Web Audio API (additive synthesis, sustain, octave shift). Play with mouse, touch, or your computer keyboard (`A`–`;`).
- **Play-along songs** — *Listen* mode lights up the keys; *Practice* mode waits for you to hit the glowing key before advancing. Public-domain tunes (Twinkle, Ode to Joy, Jingle Bells, Für Elise).
- **Chord & Scale Explorer** — pick a root + quality/scale and see it highlighted on the keyboard, hear it played or arpeggiated, and copy a shareable link.
- **Metronome** — 40–240 BPM with an accented downbeat.
- **16 lessons** — beginner → intermediate → advanced concepts, with completion tracking.
- **10 theory charts** — 7th chords, triads, the number system, circle of fifths, intervals, key signatures, pentatonic, blues, sheet music and time signatures.
- **Ear training** — note, interval and chord identification with score + streaks.
- **Practice streak** — a daily streak counter to keep you coming back.
- **Learning guides + FAQ** — long-form SEO content for beginners.

All progress (lessons completed, practice streak) is stored locally in your browser via `localStorage` — no accounts, no servers, fully private.

## 🛠️ Tech Stack

- **Single file:** `index.html` — semantic HTML, hand-written CSS, vanilla JavaScript. No build step, no framework, no dependencies.
- **Audio:** Web Audio API (`AudioContext`) — synthesized in-browser, no audio assets to load.
- **Hosting:** [Vercel](https://vercel.com/) (static), configured via `vercel.json`.

## 📁 Project Structure

```
index.html      The entire app (markup, styles, logic)
favicon.svg     Browser tab icon
og-image.png    1200×630 social share card
apple-touch-icon.png / logo.png   App icons / brand mark
sitemap.xml     Canonical sitemap
robots.txt      Crawler directives
vercel.json     Headers + SPA rewrite (modern config, no legacy routes)
```

## 🚀 Local Development

It's a static file — just serve the folder:

```bash
python -m http.server 4173
# open http://localhost:4173
```

Deploys automatically to Vercel on push to `main`.

## 💰 Monetization

- **Google AdSense** (`ca-pub-8643026289824701`) — Auto Ads enabled; manual in-content slots are wired and need their 10-digit slot IDs pasted in.
- **Amazon Associates** (`globalmx-20`) — "Recommended Gear" section with `rel="sponsored nofollow"` keyboard links.
- **Buy Me a Coffee** — support section + floating button.

## 🔎 SEO

Optimized title/description, single consolidated keyword set, canonical + hreflang, Open Graph + Twitter cards, and four JSON-LD blocks (`WebApplication`, `Organization`, `BreadcrumbList`, `FAQPage` for rich results). Google Analytics (`G-QF67XF446V`) and Search Console verification are in place.

## 📄 License

© PianoPath. Built with the Web Audio API.
