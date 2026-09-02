# Jackson's Website

Personal site built with [Astro](https://astro.build), deployed to Cloudflare Workers.

## Local development

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

Static files land in `dist/`. Cloudflare should use:

- **Build command:** `npm run build`
- **Deploy / assets:** Wrangler serves `./dist` (see `wrangler.jsonc`)

## Deploy

If your Cloudflare GitHub integration builds on push to `main`, just push.

To deploy from your machine:

```bash
npm run deploy
```
