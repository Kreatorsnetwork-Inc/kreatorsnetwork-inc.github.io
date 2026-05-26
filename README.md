# kreators-co.github.io

Client-facing reports portal for Kreators.

## URL convention

```
https://kreators-co.github.io/{category}/{client}/{yyyy-mm}-{subject}/
```

| Slot | Values |
|---|---|
| `category` | `analysis` / `proposal` / `contract` / `deck` |
| `client` | internal client code (e.g., `galaxy`, `sm`, `yg`) |
| `yyyy-mm` | ISO month |
| `subject` | lowercase, hyphenated |

## Adding a new report

1. Create folder: `{category}/{client}/{yyyy-mm}-{subject}/`
2. Drop the HTML in as `index.html`
3. Commit & push to `main`
4. Pages auto-rebuilds within ~1 min

## Notes

- Repository is **public** but `robots.txt` blocks search engine indexing.
- URL has to be shared directly with the client; not discoverable.
- For truly confidential material, request a private hosting setup separately.
