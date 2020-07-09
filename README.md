# electron-aspect-ratio-browser-window

[![npm version](https://img.shields.io/npm/v/electron-aspect-ratio-browser-window.svg?colorB=brightgreen)](https://www.npmjs.com/package/electron-aspect-ratio-browser-window)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)

Drop-in replacement for Electron's BrowserWindow with working aspect ratio on
Windows.

The module addresses this Electron issue:
https://github.com/electron/electron/issues/8036.

## Installation:

```bash
npm install --save electron-aspect-ratio-browser-window
```

## Usage:

```js
const AspectRatioBrowserWindow = require('electron-aspect-ratio-browser-window');

// AspectRatioBrowserWindow instead of BrowserWindow:
const mainWindow = new AspectRatioBrowserWindow({
    width: 800,
    height: 450
});

// Aspect ratio works on Windows, Linux, and Mac:
mainWindow.setAspectRatio(16 / 9);
```

## Try example:

```bash
cd example
npm install
npm start
```
