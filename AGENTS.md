# package-examples

pnpm monorepo with 6 single-package examples: `vlt`, `npm`, `pnpm`, `yarn`, `bun`, `deno`.

## Key Points

- Each `packages/{manager}/` is a complete, standalone starter for that package manager
- All packages use `@YOUR-ACCOUNT` placeholder (users replace with their account slug)
- Config files demonstrate minimal setup: `vlt.json` (vlt), `.npmrc` (npm/pnpm/deno), `.yarnrc.yml` (yarn), `bunfig.toml` (bun)
- Registry: `https://registry.vlt.io/YOUR-ACCOUNT/main/`

## Commands

```bash
pnpm install          # Install deps across all packages
pnpm build            # Build all packages
cd packages/npm       # Work in specific package
pnpm build            # Build single package
```
