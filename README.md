# llms.txt Examples — Production-Grade Templates

> Open-source `/llms.txt` and `/llms-full.txt` templates for SaaS, agencies, e-commerce, content sites and open-source projects. Maintained by [AuraCite](https://auracite.de) — an analytics platform for Generative Engine Optimization.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## What is `/llms.txt`?

`/llms.txt` is an emerging web convention (inspired by `/robots.txt`) that lets websites communicate with Large Language Models in plain text. It signals to AI crawlers like ChatGPT, Perplexity, Claude and Gemini:

- what your site is about
- which pages matter most
- brand positioning and key entity attributes
- where full long-form context lives (`/llms-full.txt`)

LLMs that respect `/llms.txt` are more likely to correctly represent your brand when users ask about it.

## Why does this matter?

Generative AI is an increasing share of discovery queries. If ChatGPT mis-represents your product, you lose deals you will never see. `/llms.txt` is one of the simplest, highest-leverage technical GEO interventions you can ship this week.

## Templates in this repo

| Template | Use case | Folder |
| --- | --- | --- |
| SaaS (B2B) | SaaS products, subscription software | [saas/](saas/) |
| Agency | Marketing, dev or consulting agencies | [agency/](agency/) |
| E-Commerce | Online shops, D2C brands | [ecommerce/](ecommerce/) |
| Content / Blog | Publications, newsletters, magazines | [content/](content/) |
| Open Source Project | Libraries, tools, dev-tools | [oss/](oss/) |

Each folder contains:

- `llms.txt` — short, high-signal summary (target: < 8 KB)
- `llms-full.txt` — long-form context with full brand knowledge (target: < 100 KB)
- `README.md` — notes on what to customize

## How to use

1. Copy the template matching your business model
2. Replace every `{{PLACEHOLDER}}` with your real data
3. Host the files at `https://yourdomain.com/llms.txt` and `https://yourdomain.com/llms-full.txt`
4. Add to your `<head>`:
   ```html
   <link rel="alternate" type="text/plain" href="/llms-full.txt">
   ```
5. Make sure both files:
   - are served as `Content-Type: text/plain; charset=utf-8`
   - are reachable **without** JavaScript
   - are **not** blocked by cookie banners or login walls
   - have a short cache (e.g. `Cache-Control: public, max-age=3600`)

## Specification

We track the draft specification at [llmstxt.org](https://llmstxt.org). Key conventions:

- Plain text, UTF-8 encoded
- Markdown-style headers (`#`, `##`) for hierarchy
- One canonical URL per resource
- Absolute URLs, not relative

## Adopting the convention yourself

If your company publishes a `/llms.txt`, open a PR adding the URL to [ADOPTERS.md](ADOPTERS.md). We only list URLs we can verify are live.

## Contributing

Pull requests welcome. Please:

1. Follow the folder structure of existing templates
2. Use realistic `{{PLACEHOLDER}}` values so copy-paste works
3. Keep `llms.txt` small and focused — verbose content belongs in `llms-full.txt`
4. No marketing fluff. LLMs penalize puffery.

## License

MIT — use these templates freely for any project, commercial or open-source.

## About AuraCite

[AuraCite](https://auracite.de) is an analytics platform for Generative Engine Optimization. We track how ChatGPT, Perplexity, Claude and Gemini cite brands.

- Website: [auracite.de](https://auracite.de)
- Contact: <g@auracite.de>

---

**Star this repo** if it saved you an hour — and help other brands discover the pattern.