<div align="center">

<img src="logo/nawa-light.svg" width="160" alt="NAWA" />

# NAWA Developer Platform · Documentation

### The source of [developers.trynawa.com](https://developers.trynawa.com).

Quickstart, authentication, API reference, errors, rate limits, billing, webhooks, and changelog for the NAWA platform. Powered by Mintlify, deployed automatically on push to `main`.

<br/>

![Live](https://img.shields.io/badge/live-developers.trynawa.com-0891b2?style=flat-square)
![Mintlify](https://img.shields.io/badge/built%20on-Mintlify-1A1A1A?style=flat-square)
![NAWA Green](https://img.shields.io/badge/brand-%23059669-059669?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-0a0a0a?style=flat-square)

</div>

---

## What is NAWA

AI comment management for creators. Classify intent, detect dialect, draft replies in the creator's voice. MENA-first, Arabic-native, with IBM ALLaM under the hood for Arabic.

Product: [trynawa.com](https://trynawa.com) · Docs: [developers.trynawa.com](https://developers.trynawa.com) · API gateway: [sunnybhara/nawa-api-proxy](https://github.com/sunnybhara/nawa-api-proxy)

## What's in this repo

```
.
├── introduction.mdx          ·  what NAWA is and where to start
├── quickstart.mdx            ·  first API call in five minutes
├── authentication.mdx        ·  API keys, signing, secrets
├── errors.mdx                ·  error codes + how to recover
├── billing.mdx               ·  pricing, balance, top-ups
├── changelog.mdx             ·  versioned release notes
├── api-reference/            ·  per-endpoint pages
├── guides/                   ·  long-form usage walkthroughs
├── openapi.yaml              ·  machine-readable spec
├── docs.json                 ·  Mintlify config (nav, theme, colors)
└── logo/                     ·  brand marks (light + dark) + favicon
```

## Run locally

```bash
npm install -g mint
mint dev
# → http://localhost:3000
```

Edit any `.mdx` file and the preview reloads. Sidebar order and tabs are controlled by `docs.json`.

## Deploy

Pushed to `main` triggers a Mintlify rebuild and replaces the live site. No CI to wire up in this repo; Mintlify watches the default branch.

If you need to roll back, revert the commit on `main` and Mintlify follows.

## Contributing

Small fixes (typos, broken links, clearer examples) are welcome as direct PRs. Bigger changes (a new endpoint page, a new top-level guide) should track an OpenAPI change in [`openapi.yaml`](openapi.yaml) and a CHANGELOG entry in [`changelog.mdx`](changelog.mdx). See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the conventions Mintlify expects.

## Brand

| Token | Value |
|---|---|
| Primary | `#059669` (NAWA green) |
| Secondary | `#10b981` |
| Theme | `mint`, dark by default |
| Logos | `logo/nawa-light.svg`, `logo/nawa-dark.svg` |
| Favicon | `logo/favicon.png` |

All controlled from `docs.json`. Keep the green; the cyan is reserved for secondary actions.

---

<div align="center">
<sub>Part of the NAWA platform · <a href="https://trynawa.com">trynawa.com</a></sub>
</div>
