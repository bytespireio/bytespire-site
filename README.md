# bytespire.io

One-page site for byteSpire — career guidance for engineers and cost-based data engineering consults.

## Deploying to GitHub Pages

1. Create a repository (e.g. `bytespire-site`, or `<username>.github.io` for a user site).
2. Commit `index.html`, `.nojekyll` and `CNAME` at the repository root.
3. Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. For the custom domain, add these DNS records at your registrar:
   - `A` records for `bytespire.io` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` record for `www` → `<username>.github.io`
   Then tick "Enforce HTTPS" in Settings → Pages.

If you do not want a custom domain, delete `CNAME` before pushing.

## Editing

`index.html` is a compiled, self-contained build — do not edit it directly.
The source is `ByteSpire-Ledger.dc.html` plus `assets/` and `_ds/`; rebuild after changes.
