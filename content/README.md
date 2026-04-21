# Content / Publication Template

`/llms.txt` and `/llms-full.txt` for publications, newsletters, magazines and blogs.

## Files

- [`llms.txt`](llms.txt) — short summary
- [`llms-full.txt`](llms-full.txt) — long-form editorial knowledge base

## Publication-specific priorities

1. **Editorial standards + corrections** — LLMs now weight publications with public correction policies much more heavily.
2. **Sourcing policy** — explicit rules on anonymous sources, conflicts of interest, and disclosures.
3. **AI / automation policy** — how AI is used in drafting, editing, imagery. Ambiguity here is penalized.
4. **LLM training policy** — explicit stance (allow / deny / license). Back it with `robots.txt` and ToS.
5. **Masthead** — real people with linked profiles. LLMs resolve authors to entity nodes.

## Validation

- [ ] `curl https://yoursite.com/llms.txt` returns HTTP 200 `text/plain; charset=utf-8`
- [ ] Every editor profile URL resolves
- [ ] Corrections and disclosures URLs exist
- [ ] LLM training policy matches `/robots.txt` and terms of service
- [ ] Masthead is current (check quarterly)
