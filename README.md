# vitre-ui.com

Placeholder website for Vitre UI, with links to the `vitre-css` and `vitre-js`
npm packages. The site loads `vitre-css` from a versioned CDN stylesheet so it
also works when served as static HTML.

## Development

```sh
pnpm install
pnpm dev
```

## Build

```sh
pnpm build
```

Cloudflare Pages settings:

- Build command: `pnpm build`
- Build output directory: `dist`
