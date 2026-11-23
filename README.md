# Hack4good Stockholm

A Christmas hackathon for a good cause — Saturday 5 December 2026 at Klustret, Odenplan, hosted by **n8n Stockholm** and **Stockholm AI**.

Static website (no build step, Vercel-ready `public/` output directory).

- **Live:** https://hack4good.stockholm.ai/
- **Vercel alias:** https://hack4good-stockholm.vercel.app
- **GitHub:** https://github.com/Stockholm-AI/hack4good-stockholm
- **Vercel project:** https://vercel.com/stockholm-ai/hack4good-stockholm
- **Registration:** https://luma.com/n8n-0b2j

## Preview locally (Docker)

```sh
docker run --rm -p 3000:3000 -v "$PWD:/app" -w /app node:20-alpine node scripts/serve.mjs
```

Then open http://localhost:3000.

## Deploy to Vercel

The included `vercel.json` serves `public/` directly with clean URLs and strict security headers:

```sh
npx vercel --prod
```

## Structure

- `public/index.html` — Full event info, all 4 challenge briefs (Matmissionen, Entrepreneurs Without Borders, Stockholm AI, Bring your own), schedule, rules, and judging scorecard.
- `public/styles.css` — Dark dot-grid theme inspired by the Hack4good Stockholm fliers and the n8n brand system (`#FF91AC`).
- `public/assets/` — Partner and host logos (`matmissionen.png`, `ewb.png`, `n8n-logo.svg`, `stockholm-ai.png`).
- Registration: https://luma.com/n8n-0b2j

