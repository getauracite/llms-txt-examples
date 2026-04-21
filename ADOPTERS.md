# Adopters

Live websites using `/llms.txt` and/or `/llms-full.txt` in production.

To add your site, open a pull request. We only list URLs we can verify return HTTP 200 with `Content-Type: text/plain`. The maintainers run a verification script before merging.

## Format

| Brand | URL | Template type | Verified |
| --- | --- | --- | --- |
| AuraCite | https://auracite.de/llms.txt | SaaS | pending |

## How we verify

```bash
curl -sSI https://yourdomain.com/llms.txt | head -n 5
```

The response must:

1. Return HTTP 200
2. Include `Content-Type: text/plain; charset=utf-8`
3. Be readable without JavaScript
4. Be < 50 KB for `llms.txt`

## How to submit

1. Deploy your `/llms.txt` (and optionally `/llms-full.txt`)
2. Run the verification curl above
3. Open a PR adding your row to the table
4. Link your PR to the verification output (paste response headers into the PR body)
