# AGENTS.md

## Project status
- Freshly initialized repository: no application code, `package.json`, scripts, or dependencies exist yet.
- The details below describe the **intended** stack. Verify against real files before relying on them, and update this file once code lands.

## Stack
- Vanilla HTML, CSS, and JavaScript. No framework, bundler, or TypeScript.
- Package manager: **npm**.

## Working notes for agents
- Do not assume build, test, lint, or dev scripts exist. There is no `package.json` yet, so commands like `npm test` / `npm run build` will fail — check `package.json` first and only use scripts it actually defines.
- No monorepo, CI, required services, or environment variables are configured.
- Prefer plain browser code; do not introduce a framework or build tooling unless asked.
