# What We Could Have Bought Instead

**The Price of War vs. The Cost of Home** — a data-driven comparison of U.S. Iran war spending and what that money could fund in healthcare, education, and infrastructure.

Live site: [whatwecouldhaveboughtinstead.com](https://www.whatwecouldhaveboughtinstead.com/)

## About

Operation Epic Fury costs approximately **$220 million per day** (Phase 2 sustained operations rate) — $2,546 every second. Since April 2024, the U.S. has spent an estimated **$44.1 billion** on Iran-related conflict operations.

This project puts that spending in context by showing what the same money could buy if invested domestically:

- **Healthcare**: 36,667 insulin pumps, 1.47 million therapy sessions, or 6,286 knee replacements — per day
- **Education**: 18,410 college tuitions, 2,966 teacher salaries, or 49.9 million school lunches — per day
- **Infrastructure**: 9,167 lane-miles of road maintenance, or the entire bridge repair backlog cleared in 1.5 years

All figures are estimates based on publicly available data as of March 7, 2026.

## Data Sources

The analysis draws from over 30 sources including:

- **War costs**: Brown University Costs of War Project, Al Jazeera, CSIS, IranWarCost.com, Mishpacha Magazine, JINSA
- **Healthcare**: KFF Health System Tracker, Medicare.gov, BetterCare, Healthline, SimplePractice, Soundly, GoodRx, NAMI
- **Education**: College Board, NEA, Education Data Initiative, Federal Student Aid, USDA FNS, HHS/ACF, Gordian RSMeans
- **Infrastructure**: ASCE 2025 Report Card, EPA, FHWA, Pew Charitable Trusts, NTIA, FCC

Full citations are in [`analysis.md`](analysis.md).

## Project Structure

```
index.html              — Main site (single-page, self-contained HTML/CSS/JS)
analysis.md             — Complete data analysis with all calculations and sources
og-image.png            — Open Graph / Twitter Card social image (1200×630)
favicon.ico             — Multi-size favicon (16 + 32px)
favicon-16x16.png       — 16px favicon
favicon-32x32.png       — 32px favicon
apple-touch-icon.png    — iOS home screen icon (180px)
icon-192x192.png        — Android / PWA icon
icon-512x512.png        — High-res icon / PWA splash
icon-source.svg         — Source SVG for the Split Dollar icon
```

## Deployment

The site is a single `index.html` file with no build step, no dependencies, and no JavaScript frameworks. To deploy:

1. Upload all files to any static host (Netlify, Vercel, GitHub Pages, S3, etc.)
2. Update the `og:image` and `twitter:image` meta tags with your full domain URL
3. Update the `<link rel="canonical">` tag with your production URL

## Methodology

Calculations are simple division (daily war cost ÷ unit cost = units purchasable). They do not account for supply constraints, manufacturing capacity, workforce availability, or procurement complexity. They are intended to illustrate scale, not propose literal policy alternatives.

The $220M/day sustained operations rate is derived from a phased cost model (Iran War Cost Tracker): $380M/day for initial strikes (Days 0–3), $220M/day for sustained operations (Days 3–10), and $155M/day for the air dominance/ISR phase (Day 10+). CSIS independently estimated the first 100 hours cost $3.7 billion. The model is built from seven sourced components: personnel, naval forces, aircraft operations, fuel & logistics, ordnance, C4ISR/cyber/space, and overhead. The $30M/day figure comes from comparable deployment estimates published by Mishpacha Magazine citing Brown University data.

## License

This project is open for educational and analytical use. All underlying data is from publicly available sources cited in the analysis.
