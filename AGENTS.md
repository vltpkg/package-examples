# package-examples

Single-package publishing examples — one starter for each package manager supported by vlt registry.

## Structure

Each package in `packages/` is a complete, minimal example configured for its package manager:

- **vlt** — Uses `vlt.json` for scoped registry configuration
- **npm** — Uses `.npmrc` for scoped registry configuration
- **pnpm** — Uses `.npmrc` for scoped registry configuration
- **yarn** — Uses `.yarnrc.yml` for scoped registry configuration
- **bun** — Uses `bunfig.toml` for scoped registry configuration
- **deno** — Uses `.npmrc` for scoped registry configuration

Each contains:
- `package.json` — Metadata (name, version, scripts, TypeScript dev dependency)
- `index.ts` — Simple hello-world function
- `tsconfig.json` — TypeScript configuration
- Package manager config file (vlt.json, .npmrc, .yarnrc.yml, or bunfig.toml)

## Usage

Each package serves as a starting point for the [publishing guides](https://docs.vlt.io/guides/). Users:

1. Clone a specific package directory
2. Replace `YOUR-ACCOUNT` with their vlt account slug in:
   - `package.json` (name field)
   - Package manager config file
3. Follow the publishing guide for their package manager

## Building

Install pnpm dependencies:
```bash
pnpm install
```

Build all packages:
```bash
pnpm build
```

Build a specific package:
```bash
cd packages/npm
pnpm build
```

## Configuration Notes

- All packages reference `@YOUR-ACCOUNT` as a placeholder scope
- Registry URL: `https://registry.vlt.io/YOUR-ACCOUNT/main/`
- Each config file demonstrates the minimal setup needed for that package manager
- No authentication tokens are stored in examples (users provide via environment or login)
