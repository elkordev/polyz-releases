# polyz-releases

Release artifacts for the [Polyz](https://polyz.app) desktop app.

This repo holds only the built binaries (dmg/zip/blockmaps) and `latest-mac.yml` auto-update manifest. **No source code lives here** — source is in a separate private repo. The landing site at polyz.app proxies downloads from this repo via a server-side token; this repo never needs to be public for users to install.

Releases are produced by `npm run release` from the source repo.
