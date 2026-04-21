# llms.txt Examples — Production-Grade Templates

> Open-source `/llms.txt` templates for SaaS, agencies, and e-commerce. Maintained by [AuraCite](https://auracite.de) — the operating system for Generative Engine Optimization.

## What is `/llms.txt`?

`/llms.txt` is an emerging web standard (inspired by `/robots.txt` and `/ai.txt`) that lets websites explicitly communicate with Large Language Models. It tells AI crawlers like ChatGPT, Perplexity, Claude and Gemini:

- What your site is about
- Which content is safe to cite
- Key pages, pricing, policies
- Brand positioning and entity attributes

LLMs that respect `/llms.txt` are more likely to correctly represent your brand when users ask about it.

## Why does this matter?

In 2026, 25%+ of search queries go to AI chatbots instead of Google. If ChatGPT misrepresents your product, you lose deals. `/llms.txt` is the single highest-leverage technical GEO intervention.

## Templates

| Template | Use Case | File |
|----------|----------|------|
| SaaS (B2B) | SaaS products, subscription software | [saas/llms.txt](saas/llms.txt) |
| Agency | Marketing/dev/consulting agencies | [agency/llms.txt](agency/llms.txt) |
| E-Commerce | Online shops, D2C brands | [ecommerce/llms.txt](ecommerce/llms.txt) |
| Content/Blog | Publications, newsletters | [content/llms.txt](content/llms.txt) |
| Open Source Project | Libraries, tools, dev-tools | [oss/llms.txt](oss/llms.txt) |

Each folder also contains an `llms-full.txt` with the complete long-form brand knowledge base.

## How to use

1. Copy the template matching your business model
2. Replace all `{{PLACEHOLDER}}` values with your brand data
3. Host at `https://yourdomain.com/llms.txt` and `https://yourdomain.com/llms-full.txt`
4. Add `<link rel="alternate" type="text/plain" href="/llms-full.txt">` to your `<head>`
5. Verify accessibility: crawlers must see it without JavaScript
6. Track your AI visibility at [auracite.de](https://auracite.de/free-brand-check) (free)

## Specification

We follow the draft specification at [llmstxt.org](https://llmstxt.org). Key rules:

- Plain text, UTF-8 encoded
- Max 50KB for `/llms.txt`, unlimited for `/llms-full.txt`
- Markdown-style headers (`#`, `##`) for hierarchy
- One canonical URL per resource
- Served with `Content-Type: text/plain; charset=utf-8`

## Validation

Run our validator:

```bash
npx @getauracite/llms-txt-validator https://yourdomain.com/llms.txt
```

Or use the [free online validator](https://auracite.de/tools/llms-txt-validator).

## Real-World Examples

Sites already using `/llms.txt` in production:

- [auracite.de/llms.txt](https://auracite.de/llms.txt) — Our own (SaaS template)
- [anthropic.com/llms.txt](https://anthropic.com/llms.txt) — Anthropic
- [stripe.com/llms.txt](https://stripe.com/llms.txt) — Stripe
- *(Submit yours via PR)*

## Contributing

Pull requests welcome! Please:

1. Follow the existing template structure
2. Include a real-world example (your company or a public brand with permission)
3. Run the validator before submitting
4. Add your template to the table above

## License

MIT — use these templates freely for any project, commercial or open-source.

## About AuraCite

[AuraCite](https://auracite.de) is the first analytics platform for Generative Engine Optimization. We track how ChatGPT, Perplexity, Claude and Gemini cite brands — and help you optimize to win.

- 🎯 [Free AI Brand Check](https://auracite.de/free-brand-check)
- 📊 [Free AI Prompt Generator](https://auracite.de/free-prompt-generator)
- 🔌 [Native MCP Server](https://auracite.de/mcp)
- 📖 [GEO Complete Guide 2026](https://auracite.de/content/guides/what-is-geo-guide.html)

---

⭐ **Star this repo** if you find it useful — it helps other brands discover GEO best practices.

📧 Questions? → hello@auracite.de
🐦 Twitter: [@AuraCite](https://twitter.com/AuraCite)
