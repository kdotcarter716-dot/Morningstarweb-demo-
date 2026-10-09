# Morningstarweb-demo-

A one-page site for an **invented** business ("Sample Cafe"), published here to prove that
MORNING STAR WEB can put a page on public hosting and reach it over HTTPS.

It is not a real company, and no real business is a customer of ours. The page says so itself.

**Live:** https://kdotcarter716-dot.github.io/Morningstarweb-demo-/

## How a customer's site gets delivered this way

1. Put the finished page at `index.html` in the repo root (plus any images alongside it).
2. Commit and push to `main`.
3. GitHub Pages serves it. Pages is enabled per repo: Settings -> Pages -> "Deploy from a branch",
   branch `main`, folder `/ (root)`. (`.nojekyll` is here so the files are served exactly as-is.)
4. **A customer's own domain:** add a file named `CNAME` in the repo root containing the domain,
   then point that domain's DNS at GitHub Pages:
   - `www` -> `CNAME` -> `kdotcarter716-dot.github.io`
   - bare domain -> the four GitHub Pages `A` records
   Then tick "Enforce HTTPS" in the repo's Pages settings (the certificate is issued automatically).

For a real customer, use a separate repo per customer (e.g. `msweb-client-<name>`) so their page,
and later their domain, stay independent of everyone else's.

## Cost

Free — GitHub Pages on a public repo costs nothing and does not need a card, so it adds nothing to
a $100 Starter build or a $30/month plan.
