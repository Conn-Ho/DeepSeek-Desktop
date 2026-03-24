# DeepSeek Desktop

> DeepSeek AI wrapped as a native desktop app using Electron. Clean, minimal, no browser tabs.

A lightweight Electron wrapper that turns [DeepSeek Chat](https://chat.deepseek.com/) into a standalone macOS / Windows / Linux desktop application — no browser clutter, no tab juggling.

## Features

- **Native window** — dedicated app with a clean interface, no browser toolbar
- **macOS-native behavior** — stays open in the Dock when all windows are closed
- **Cross-platform builds** — DMG (macOS), NSIS installer (Windows), AppImage (Linux)
- **No menu bar** — distraction-free chat experience

## Tech Stack

| | |
|---|---|
| Runtime | Electron 28 |
| Packager | electron-builder |
| Target URL | chat.deepseek.com |

## Quick Start

```bash
npm install
npm start
```

## Build

```bash
# macOS DMG
npm run build -- --mac

# Windows installer
npm run build -- --win

# Linux AppImage
npm run build -- --linux
```

Output goes to `dist/`.

## Note

This app loads `chat.deepseek.com` in a sandboxed Electron window. Node integration is disabled. No data is collected or proxied — it is a thin native shell over the official DeepSeek web interface.
