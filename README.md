![vlt](https://github.com/user-attachments/assets/aec7c817-b83f-4d71-b34a-4e480b97e82c)

# package-examples

Single-package examples for publishing — one starter for each package manager.

Each package is a simple TypeScript "hello world" package configured for its respective package manager and vlt registry.

## Packages

- **[vlt](./packages/vlt)** — Example using vlt
- **[npm](./packages/npm)** — Example using npm
- **[pnpm](./packages/pnpm)** — Example using pnpm
- **[yarn](./packages/yarn)** — Example using yarn
- **[bun](./packages/bun)** — Example using bun
- **[deno](./packages/deno)** — Example using deno

## Structure

Each package contains:

- `index.ts` — Simple hello-world TypeScript function
- `package.json` — Package metadata (name, version, scripts, dependencies)
- `tsconfig.json` — TypeScript configuration
- Package manager config file (`vlt.json`, `.npmrc`, `.yarnrc.yml`, `bunfig.toml`, etc.)

## Usage

Each package can be used as a starting point for the [publishing guides](https://docs.vlt.io/guides/).

Clone a specific package directory or explore locally:

```bash
pnpm install
pnpm build
```

## Development

Install dependencies:

```bash
pnpm install
```

Build all packages:

```bash
pnpm build
```
