# vitre-ui.com

![Vitre UI](https://vitre-ui.com/images/vitre-ui-dark.webp)

Landing page for Vitre UI. It states what the library is, shows the two lines
needed to use it, and links to the documentation, components, the examples
kitchen sink, the source repository, and npm.

The site loads `vitre.css` from an unpkg CDN stylesheet so it also works when
served as static HTML. It uses no class names of its own: page-specific styles
in `src/site.css` hang off `data-*` attributes, matching Vitre's conventions,
and everything else is Vitre's default element styling.

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
