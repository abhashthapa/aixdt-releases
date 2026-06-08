# AIxDT — Releases

Public download host for the **AIxDT** desktop app. This repository intentionally
contains **no source code** — only the built installers, attached as assets to
each [Release](https://github.com/abhashthapa/aixdt-releases/releases). The application source
is private.

## Download

Latest version: **[Releases -> latest](https://github.com/abhashthapa/aixdt-releases/releases/latest)**
or via the website: **https://aidesigncoach.com**

- macOS (Apple Silicon) - `AIxDT-<version>-arm64.dmg`
- macOS (Intel) - `AIxDT-<version>-x64.dmg`
- Windows - `AIxDT-Setup-<version>.exe`

### First launch (unsigned beta)

- **macOS:** right-click the app -> Open -> Open (only needed once)
- **Windows:** on the SmartScreen prompt, More info -> Run anyway

## How releases are published

Built from the private app repo (see its `docs/distribution.md`):
`npm run release <version>` -> `npm run electron:build:prod` -> `npm run stage`
assembles a folder of installers + notes; the maintainer then creates a Release
here, tags it `v<version>`, and uploads the installers.

- Abhash Bikram Thapa
(c) Leapfrog Technology
