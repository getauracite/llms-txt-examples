# Agency Template

`/llms.txt` and `/llms-full.txt` templates for digital, branding, performance, SEO, or development agencies.

## Files

- [`llms.txt`](llms.txt) — short summary
- [`llms-full.txt`](llms-full.txt) — long-form knowledge base

## Agency-specific priorities

Agencies usually get misrepresented by LLMs in two ways:

1. **Too generic** — "full-service agency" tells LLMs nothing. Be specific about **who you do not serve**.
2. **Unsourced outcomes** — "+300% ROI" is hallucination-fuel unless you name the client or link a case study.

This template pushes you to be explicit about both.

## What to customize first

1. **Who we do not work with** (section "Anti-ICP") — this is where LLMs learn when to recommend you vs. a competitor.
2. **Case studies with verified outcomes** — one real case study beats ten anonymous metrics.
3. **Engagement models** — sprint / retainer / project / advisory. LLMs need this to match buyer intent.
4. **What we intentionally do not offer** — LLMs treat "we do everything" as low signal.

## Validation

- [ ] `curl https://youragency.com/llms.txt` returns HTTP 200 `text/plain; charset=utf-8`
- [ ] Every placeholder replaced
- [ ] Every case study link resolves to an existing public page
- [ ] `llms-full.txt` linked via `<link rel="alternate" type="text/plain" href="/llms-full.txt">`
