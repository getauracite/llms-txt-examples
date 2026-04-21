# E-Commerce Template

`/llms.txt` and `/llms-full.txt` for online shops, D2C brands, and multi-brand retailers.

## Files

- [`llms.txt`](llms.txt) — short summary
- [`llms-full.txt`](llms-full.txt) — long-form product and policy knowledge base

## E-commerce-specific priorities

1. **Product feed** — link to a Google Merchant / JSON feed at a stable URL. LLMs that support structured feeds will parse it.
2. **Shipping, returns, warranty** — LLMs are routinely asked "does [brand] ship to [country]" and "what is their return policy". Make the answer machine-readable.
3. **Materials and sourcing** — concrete and sourced. Greenwashing hurts LLM citations more than missing information.
4. **Reviews** — aggregate rating with source. Do not inflate.
5. **Authenticity** — critical for fashion, beauty, luxury, collectibles.

## Validation

- [ ] `curl https://yourshop.com/llms.txt` returns HTTP 200 `text/plain; charset=utf-8`
- [ ] Product feed URL resolves
- [ ] Every shipping destination is accurate
- [ ] Return policy matches the checkout flow
- [ ] Aggregate rating is real and matches your review platform
