# electron-aspect-ratio-browser-window

Drop-in replacement for Electron's BrowserWindow with working aspect ratio on
Windows.

The module addresses this Electron issue:
https://github.com/electron/electron/issues/8036.

## Usage:

```js
const AspectRatioBrowserWindow = require('electron-aspect-ratio-browser-window');

// AspectRatioBrowserWindow instead of BrowserWindow:
const mainWindow = new AspectRatioBrowserWindow({
    width: 800,
    height: 450
});

mainWindow.setAspectRatio(16 / 9);
```

## Try example:

```bash
cd example
npm install
npm start
```
