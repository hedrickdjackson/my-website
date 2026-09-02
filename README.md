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

Static files land in `dist/`.

## Cloudflare Workers Builds

In the Worker **Settings → Build**, use:

| Setting | Value |
| --- | --- |
| **Build command** | `npm run build` |
| **Deploy command** | `npx wrangler deploy` |

Without the build command, deploy fails because `dist/` does not exist yet. Wrangler serves `./dist` (see `wrangler.jsonc`).

## Deploy locally

```bash
npm run deploy
```
