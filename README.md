# 💰 Treasury — Personal Budget Tracker

> A beautiful, AI-powered personal finance app that lives on your iPhone home screen.

![License](https://img.shields.io/badge/license-MIT-gold) ![PWA](https://img.shields.io/badge/PWA-ready-brightgreen) ![Offline](https://img.shields.io/badge/offline-supported-blue)

---

## ✨ Features

- **Dashboard** — Income, expenses, payments, and net balance at a glance with charts
- **Expense Tracker** — Log daily spending by category with dates
- **Recurring Payments** — Track bills and subscriptions with due-date alerts
- **Budget Manager** — Set monthly limits per category with visual progress bars
- **AI Financial Advisor** — Powered by Claude, gives personalized advice based on your actual data
- **Offline Support** — Works without internet after first load
- **100% Private** — All data stored locally on your device, nothing sent to any server

---

## 📱 Install on iPhone

1. Open this page in **Safari** (not Chrome)
2. Tap the **Share button** at the bottom of the screen
3. Tap **"Add to Home Screen"**
4. Tap **Add** — Treasury will appear on your home screen like a native app

---

## 🤖 Enable the AI Advisor

The AI Advisor uses the Anthropic Claude API. To enable it:

1. Go to [console.anthropic.com](https://console.anthropic.com) and create an account
2. Generate an API key
3. Open Treasury → tap **Settings** → paste your key → tap **Save**

Your API key is stored only on your device and never leaves it.

---

## 🚀 Deploy Your Own

This is a zero-dependency PWA — three files, no build step needed.

### GitHub Pages (recommended)
1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch
4. Your app will be live at `https://YOUR-USERNAME.github.io/treasury`

### Any static host
Upload `index.html`, `manifest.json`, and `sw.js` to any static hosting service:
- [Netlify](https://netlify.com) — drag & drop deploy
- [Vercel](https://vercel.com) — connect GitHub repo
- [Cloudflare Pages](https://pages.cloudflare.com)

---

## 🗂 File Structure

```
treasury/
├── index.html      # The entire app (HTML + CSS + JS)
├── manifest.json   # PWA configuration (name, icon, colors)
├── sw.js           # Service worker for offline support
└── README.md       # This file
```

---

## 🔒 Privacy

- **No backend.** There is no server, database, or analytics.
- **No accounts.** Nothing to sign up for.
- **Local storage only.** Your financial data lives in your browser's local storage on your device.
- **API calls go directly** from your browser to Anthropic when using the AI Advisor. Your financial summary is sent to generate advice — review [Anthropic's privacy policy](https://www.anthropic.com/privacy) for details.

---

## 🛠 Tech Stack

- Vanilla HTML, CSS, and JavaScript — no frameworks, no bundler
- Progressive Web App (PWA) with service worker caching
- SVG-based charts (no charting library)
- [Anthropic Claude API](https://anthropic.com) for AI advice
- Google Fonts (Playfair Display + DM Sans)

---

## 📄 License

MIT — do whatever you want with it.
