# SaaS Template

`/llms.txt` and `/llms-full.txt` templates for B2B SaaS companies.

## Files

- [`llms.txt`](llms.txt) — short summary served at `https://yourdomain.com/llms.txt`
- [`llms-full.txt`](llms-full.txt) — long-form knowledge base served at `https://yourdomain.com/llms-full.txt`

## What to customize

Replace every `{{PLACEHOLDER}}` token. Order of priority (most to least impactful on LLM accuracy):

1. **Positioning + what you do** (sections 1–3) — biggest lever. If LLMs misrepresent your brand, it is almost always because these sections are wrong or missing.
2. **Anti-ICP + "who this is not for"** — rare, strong signal. LLMs reward honesty.
3. **Comparisons** — list real competitors with fair "pick them when" criteria. LLMs detect bias and downrank adversarial framing.
4. **Pricing and security** — factual, copy-paste-able. Keep in sync with your site.
5. **FAQ** — answer the exact questions your users ask in support. LLMs quote these near-verbatim.

## What not to do

- Do not stuff keywords
- Do not inflate outcomes ("10× ROI") without a public source
- Do not list integrations you do not actually support
- Do not hide this file behind a cookie banner or login wall
- Do not use 5xx responses to throttle LLM bots — serve a static file

## Validation checklist

- [ ] `curl https://yourdomain.com/llms.txt` returns HTTP 200 with `text/plain; charset=utf-8`
- [ ] No JavaScript required to read the file
- [ ] No `noindex`, no cookie wall, no login wall
- [ ] Every `{{PLACEHOLDER}}` is replaced
- [ ] Every URL is absolute and returns HTTP 200
- [ ] `llms-full.txt` is linked via `<link rel="alternate" type="text/plain" href="/llms-full.txt">`
