# DataSaver NG — Website 🇳🇬

> Official landing page for [DataSaver NG](https://datasaver-ng.vercel.app) — Nigeria's #1 data saving Chrome extension.

---

## About

This repo contains the landing page website for DataSaver NG. Built with pure HTML, CSS, and vanilla JavaScript — no build tools, no frameworks, instant deploy.

**Live site:** [datasaver-ng-website.vercel.app](https://datasaver-ng-website.vercel.app)

---

## Related Repos

| Repo | Description | Link |
|------|-------------|-------|
| datasaver-ng | Proxy server + Chrome extension | [github.com/Zenskistudios/datasaver-ng](https://github.com/Zenskistudios/datasaver-ng) |

---

## What the Landing Page Shows

- Live data savings pulled from the proxy API in real time
- How DataSaver NG works (4 saving methods explained)
- Data savings breakdown by category
- 4-step install guide
- FAQ built specifically for Nigerian users (MTN, Airtel, Glo, 9mobile)
- Direct link to Chrome Web Store

---

## Files

```
datasaver-ng-website/
├── index.html    ← The entire landing page (single file)
└── README.md     ← This file
```

---

## Local Development

No build tools needed. Just open in browser:

```bash
git clone https://github.com/Zenskistudios/datasaver-ng-website
cd datasaver-ng-website
# Open index.html in Chrome
```

Or use VS Code Live Server extension for hot reload.

---

## Deployment

Auto-deploys to Vercel on every push to `main`.

Manual deploy:
```bash
npm i -g vercel
vercel --prod
```

---

## How the Live Stats Work

The landing page fetches real-time data from the proxy server:

```javascript
fetch('https://datasaver-ng.vercel.app/stats')
  .then(r => r.json())
  .then(data => {
    // Updates MB saved and requests counters live
  });
```

---

## Roadmap

- [x] Landing page with live stats
- [x] How it works section
- [x] Install guide
- [x] Nigerian-specific FAQ
- [ ] Migrate to Next.js for better SEO
- [ ] Add user testimonials
- [ ] Add changelog page
- [ ] Add blog for data saving tips

---

## Built By

Built in Lagos, Nigeria 🇳🇬 by [@Zenskistudios](https://github.com/Zenskistudios)

*Your data, your money, protected.*
