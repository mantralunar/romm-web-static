# RomM Web Static

Automatically builds the static RomM frontend from official RomM releases.

Upstream project:

https://github.com/rommapp/romm

## How it works

This repository periodically checks the latest stable RomM release.

When a new version is detected, GitHub Actions:

1. Checks out the matching RomM release tag
2. Installs the frontend dependencies
3. Builds the RomM Vue/Vite frontend
4. Packages the generated static files
5. Publishes them as a GitHub Release

No RomM source code is stored in this repository.

## Release files

Each release contains:

```text
romm-web-static-VERSION.tar.gz
romm-web-static.tar.gz
romm-web-static-VERSION.tar.gz.sha256
