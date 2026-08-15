# vitre-ui.com

![Vitre UI](https://vitre-ui.com/images/vitre-ui-dark.webp)

Landing page for Vitre UI, linking to the documentation, the component
reference, the `vitre-css` npm package, and the GitHub repository. The site
loads `vitre.css` from an unpkg CDN stylesheet so it also works when served as
static HTML.

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
