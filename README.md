# kreatorsnetwork-inc.github.io

Client-facing reports portal for Kreators.

## URL convention

```
https://kreatorsnetwork-inc.github.io/{category}/{client}/{yyyy-mm}-{subject}-{tier}/
```

| Slot | Values |
|---|---|
| `category` | `analysis` / `proposal` / `contract` / `deck` |
| `client` | internal client code (e.g., `galaxy`, `sm`, `yg`) |
| `yyyy-mm` | ISO month |
| `subject` | lowercase, hyphenated |
| `tier` | `masked` (pre-contract teaser) / `full` (post-contract full report) |

## Two-tier delivery flow

1. **`-masked`** — initial proposal sent to prospect. Key numbers redacted/blurred. URL shared to drive contract signature.
2. **`-full`** — unmasked full report, delivered only **after** initial contract signed. Same `{subject}` slug, only the tier suffix changes.

Example pair:
- `analysis/galaxy/2026-05-taemin-us-masked/` ← shared pre-signature
- `analysis/galaxy/2026-05-taemin-us-full/`   ← shared post-signature

## Adding a new report

1. Create folder: `{category}/{client}/{yyyy-mm}-{subject}/`
2. Drop the HTML in as `index.html`
3. Commit & push to `main`
4. Pages auto-rebuilds within ~1 min

## Notes

- Repository is **public** but `robots.txt` blocks search engine indexing.
- URL has to be shared directly with the client; not discoverable.
- For truly confidential material, request a private hosting setup separately.
