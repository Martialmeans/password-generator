# AGENTS.md

## Project
- Single-file password generator web app: `index.html` (HTML + CSS + vanilla JS, no dependencies).
- Built in phases; Phase 1 (core generator) is done. Open `index.html` directly in a browser to run it — no build or dev server. `crypto.getRandomValues` works on `file://`.
- Package manager: **npm**, but there is still no `package.json`. Do not assume build/test/lint/dev scripts exist — check for `package.json` first and only run scripts it defines.
- Rules for this app: use `crypto.getRandomValues()` (never `Math.random()`) with rejection sampling; never log/store/send generated passwords.

## Git & GitHub
- `git` (2.56) and `gh` (2.102) are installed and on the system PATH — a fresh terminal resolves both normally.
- Only if a shell reports "git is not recognized" (it inherited a stale PATH, e.g. a session started before a PATH change), prepend: `$env:PATH = "C:\Program Files\Git\cmd;" + $env:PATH` (gh dir: `C:\Program Files\GitHub CLI`).
- Remote `origin` = https://github.com/Martialmeans/password-generator.git (public). Default/pushed branch is `master` (not `main`).
- `git push`/`gh` write progress to stderr; PowerShell may render this as a red `NativeCommandError` even when the command succeeded — verify with `git status -sb`.
