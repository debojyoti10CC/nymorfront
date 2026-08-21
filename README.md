<p align="center">
  <img src="public/logo/light.png" alt="Nymor" width="72" />
</p>

<h1 align="center">nymorfront</h1>

The marketing/landing page for [Nymor](https://github.com/debojyoti10CC/nymor) — a static site with no wallet connections, no live API calls, no backend. Every number and claim on the page is a fixed, verified fact (a real transaction hash, a real test count) checked against the actual project before shipping, not fetched live.

Its whole job is to explain what Nymor is and point people to the two places with real depth:

- **[docs.nymor.xyz](https://docs.nymor.xyz/)** — architecture, the on-chain policy deep dive, and the honest status of every component.
- **[github.com/debojyoti10CC/nymor](https://github.com/debojyoti10CC/nymor)** — the actual source.

## Design

Plain Vite, no framework — a single `index.html` plus `src/style.css`. The visual system (serif/sans/mono type stack via bundled `EB Garamond` + `Geist` + `Geist Mono`, diagonal-stripe body background, bordered fixed-width shell, light/dark via `prefers-color-scheme`) is shared with [`wardfront`](../wardfront), swapped from teal to Nymor's red.

## Running

```bash
npm install
npm run dev       # :5175
npm run build
```

## Keeping the numbers honest

Every stat on this page (test counts, transaction hashes, resource counts) should be re-verified against the `nymor` repo before updating this site — don't just bump a number because it sounds better. `npm run build` doesn't check this for you.
