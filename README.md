# polyz-releases

Public release artifacts for the [Polyz](https://polyz.app) desktop app.

Holds the built installers (`dmg`/`exe`), auto-update `zip`s + blockmaps,
and the `latest-mac.yml` / `latest.yml` update manifests. **No source code
lives here** — source is in a separate private repo.

This repo is **public** so `electron-updater` and direct downloads can fetch
releases anonymously. The app is gated at **runtime**, not at download:
using it requires a signed-in account with an active subscription or trial,
so a freely-obtained binary is unusable (no new writing, no AI, no sync)
without a paid plan.

Releases are produced by `npm run release` from the source repo (macOS:
built, signed, and notarized locally) plus the Windows CI workflow.