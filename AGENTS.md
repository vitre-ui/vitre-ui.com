# Repository Guidelines

## Project Structure & Module Organization

This repository currently contains a minimal website scaffold:

- `README.md` describes the project.
- `AGENTS.md` provides contributor and agent guidance.

When adding implementation files, keep the layout predictable. Place source under `src/`, static assets under `public/` or `assets/`, and tests near the code they cover or under `tests/`. Example paths: `src/components/Header.tsx`, `public/favicon.svg`, `tests/homepage.test.ts`.

## Build, Test, and Development Commands

No package manager, framework, or build scripts are committed yet. Before adding commands, commit the relevant manifest, such as `package.json` and a lockfile.

Recommended command names once tooling exists:

- `npm run dev` or `pnpm dev`: start the local development server.
- `npm run build` or `pnpm build`: create the production build.
- `npm test` or `pnpm test`: run the automated test suite.
- `npm run lint` or `pnpm lint`: run style and static checks.

Document new commands in `README.md` when introduced.

## Coding Style & Naming Conventions

Follow the conventions of the framework added to the project. Until formatter configuration exists, use 2-space indentation for web files, descriptive file names, and clear module names.

Suggested naming patterns:

- Components: `PascalCase`, such as `SiteHeader.tsx`.
- Utilities and hooks: `camelCase`, such as `formatTitle.ts` or `useNavigation.ts`.
- Static assets: lowercase kebab-case, such as `brand-mark.svg`.

Add formatter and lint configuration with the first substantial source contribution.

## Testing Guidelines

No test framework is configured yet. When adding behavior, add tests with the chosen stack and make them runnable with one command, such as `npm test`.

Use test names that describe user-visible behavior, for example `homepage renders primary navigation`. Keep tests close to the feature, such as `src/components/Header.test.tsx`, or use `tests/` for integration coverage.

## Commit & Pull Request Guidelines

The current Git history only contains `Initial commit`, so no project-specific convention is established. Use short, imperative subjects, such as `Add homepage scaffold`.

Pull requests should include:

- A concise summary of the change.
- Any commands run, such as `npm test`.
- Screenshots or recordings for visible UI changes.
- Linked issues or context when applicable.

Keep pull requests focused. Separate infrastructure, design, and content changes when practical.

## Agent-Specific Instructions

Do not assume hidden build tooling exists. Inspect the repository before editing, keep changes narrowly scoped, and update this guide when new project structure, commands, or conventions are added.
