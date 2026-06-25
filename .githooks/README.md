# Git hooks for this repo

This is the **public** Nexus downloads repository. It must contain **only
documentation** — the app installers are published as **GitHub Release assets**,
never committed here.

The `pre-commit` hook refuses any commit that adds source code or build/config
files, so source can never accidentally leak into this public repo.

## Enabling the hook

Git does not install hooks automatically on clone. Run this **once per clone**:

```sh
git config core.hooksPath .githooks
```

(It is already enabled in the clone where this repo was set up.)

## What gets blocked

Anything that looks like application source or build config — e.g. `.rs`, `.ts`,
`.tsx`, `.js`, `.sql`, `.sh`, `Cargo.toml`, `package.json`, `Dockerfile`,
`tauri.conf.json`, `.env*`, etc. Markdown, text, and images are allowed.

## Bypassing

Only if a genuine documentation file is misflagged:

```sh
git commit --no-verify
```
