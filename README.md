# Commerce Platform Core

A commerce backend platform snapshot with core packages, dashboard packages, docs, and extensibility tooling.

## Features

- Commerce API and core packages
- Admin/dashboard package workspace
- GraphQL schemas and code generation
- Plugin-oriented architecture
- Documentation and end-to-end testing assets

## Tech stack

- TypeScript
- Node.js
- GraphQL
- Angular
- React
- Bun
- Lerna

## Screenshots

Screenshots are not included in this repository snapshot. Run the app locally and add current product screenshots when a deployment is available.

## Installation

Use the package manager indicated by the lockfile in this repository. Install from the repository root before running app-specific commands.

## Environment variables

Create local environment files from the example files included in the repository, or start from this root example:

| Variable | Purpose |
| --- | --- |
| `APP_ENV` | Configure for the local or deployed environment. |
| `COOKIE_SECRET` | Configure for the local or deployed environment. |
| `SUPERADMIN_USERNAME` | Configure for the local or deployed environment. |
| `SUPERADMIN_PASSWORD` | Configure for the local or deployed environment. |
| `DB_HOST` | Configure for the local or deployed environment. |
| `DB_PORT` | Configure for the local or deployed environment. |
| `DB_NAME` | Configure for the local or deployed environment. |
| `DB_USERNAME` | Configure for the local or deployed environment. |
| `DB_PASSWORD` | Configure for the local or deployed environment. |

## Development commands

```bash
bun install
```
```bash
bun run build
```
```bash
bun run test
```
```bash
bun run lint
```
```bash
bun run docs:build
```

## Build and deploy notes

- Review the included Docker, compose, or package-specific deployment files before production use.
- Keep secrets outside git and provide them through the deployment platform or local untracked environment files.
- For large workspace builds, run package-specific checks first, then the root build command.

## Project structure

- `docker-compose.yml`
- `docs/` — project directory
- `e2e-common/` — project directory
- `license/` — project directory
- `LICENSE.md`
- `NOTICE.md`
- `package.json`
- `packages/` — project directory
- `scripts/` — project directory

## Verification status

This public snapshot was prepared with dependency directories, generated output, local editor settings, and private environment files removed. See `PUBLISHING_REPORT.md` for the exact safety and verification checks run before publication.

## License

MIT as included in LICENSE.md. Preserve the included license and notice files when redistributing.

## Author

gotowebevents <info@gotowebevents.com>
