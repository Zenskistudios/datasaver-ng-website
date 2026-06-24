# DataSaver NG — Landing Page 🇳🇬

> Official website for [DataSaver NG](https://datasaver-ng.vercel.app) — the data saving Chrome extension built for Nigerian internet users.

## What is DataSaver NG?

DataSaver NG is a Chrome extension that physically reduces how much data your browser downloads — compressing images, blocking trackers, and stripping ad scripts before they reach you. Built specifically for Nigerian users on MTN, Airtel, Glo, and 9mobile.

## This Repo

This repo contains the landing page website for DataSaver NG. It is a single `index.html` file deployed on Vercel.

**Live site:** coming soon

## Related Repos

| Repo | Description |
|------|-------------|
| [datasaver-ng](https://github.com/Zenskistudios/datasaver-ng) | Proxy server (Node.js) deployed on Vercel |

## How the Product Works

```
[Your Browser]
     ↓
[DataSaver NG Extension]
     ↓  blocks trackers via declarativeNetRequest
     ↓  routes images through proxy
[Proxy Server — datasaver-ng.vercel.app]
     ↓  compresses images to WebP (60% quality)
     ↓  strips tracking scripts from HTML
     ↓  gzip compresses all responses
[Website — loads faster, uses less data]
```

## Features

- Compresses images by up to 70% using WebP conversion
- Blocks 15+ trackers (Google Analytics, Facebook Pixel, Taboola, etc.)
- Strips ad scripts and tracking pixels from HTML pages
- Shows live data savings in the extension popup
- Works on all Nigerian networks — MTN, Airtel, Glo, 9mobile
- Free forever — no account, no subscription

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Landing page | HTML, CSS, vanilla JS |
| Chrome extension | JavaScript (Manifest V3) |
| Proxy server | Node.js + Express |
| Image compression | Sharp (WebP) |
| HTML parsing | Cheerio |
| Hosting | Vercel (free tier) |

## Local Development

No build tools needed. Just open `index.html` in your browser:

```bash
git clone https://github.com/Zenskistudios/datasaver-ng-website
cd datasaver-ng-website
open index.html
```

## Deployment

This site auto-deploys to Vercel on every push to `main`.

To deploy manually:
1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel --prod`

## Contributing

Pull requests are welcome. If you find a bug or want to improve the landing page, open an issue first to discuss what you'd like to change.

## Roadmap

- [ ] Publish extension to Chrome Web Store
- [ ] Android app with VPN tunnel for all-app data saving
- [ ] User accounts and data saving history
- [ ] Network-aware mode (auto-adjust quality on 2G vs 4G)
- [ ] Firefox extension support

## Built By

Built in Lagos, Nigeria 🇳🇬 by [@Zenskistudios](https://github.com/Zenskistudios)

---

*Your data, your money, protected.*
