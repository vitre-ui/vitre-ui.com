# Repository Guidelines

## Project Structure & Module Organization

This repository contains a minimal Vite website:

- `README.md` describes the project.
- `AGENTS.md` provides contributor and agent guidance.
- `index.html` is the Vite entry point and contains the placeholder page.
- `src/main.js` imports `vitre-css` and local site styles.
- `src/site.css` contains the small amount of page-specific CSS.
- `public/images/` contains static image assets served from `/images/...`.

When adding implementation files, keep the layout predictable. Place source under `src/` if the site grows, static assets under `public/`, and tests near the code they cover or under `tests/`.

## Build, Test, and Development Commands

Use pnpm with the committed Vite scripts:

- `pnpm install`: install dependencies.
- `pnpm dev`: start the local Vite development server.
- `pnpm build`: create the production build in `dist/`.
- `pnpm preview`: preview the built site locally.

Document new commands in `README.md` when introduced.

## Coding Style & Naming Conventions

Follow the conventions of the framework added to the project. Until formatter configuration exists, use 2-space indentation for web files, descriptive file names, and clear module names.

Suggested naming patterns:

- Components: `PascalCase`, such as `SiteHeader.tsx`.
- Utilities and hooks: `camelCase`, such as `formatTitle.ts` or `useNavigation.ts`.
- Static assets: lowercase kebab-case, such as `brand-mark.svg`.

Add formatter and lint configuration with the first substantial source contribution.

## Testing Guidelines

No test framework is configured yet. When adding behavior, add tests with the chosen stack and make them runnable with one command, such as `pnpm test`.

Use test names that describe user-visible behavior, for example `homepage renders primary navigation`. Keep tests close to the feature, such as `src/components/Header.test.tsx`, or use `tests/` for integration coverage.

## Commit & Pull Request Guidelines

The current Git history only contains `Initial commit`, so no project-specific convention is established. Use short, imperative subjects, such as `Add homepage scaffold`.

Pull requests should include:

- A concise summary of the change.
- Any commands run, such as `pnpm test`.
- Screenshots or recordings for visible UI changes.
- Linked issues or context when applicable.

Keep pull requests focused. Separate infrastructure, design, and content changes when practical.

## Deployment

Cloudflare Pages should use `pnpm build` as the build command and `dist` as the output directory. Static assets in `public/` are copied to `dist/` by Vite and should be referenced from root-relative paths such as `/images/vitre-ui-dark.webp`.

## Agent-Specific Instructions

Inspect the repository before editing, keep changes narrowly scoped, and update this guide when new project structure, commands, or conventions are added.
