# ShinX ScriptHub

A modern, lightweight ScriptHub built with pure **HTML, CSS, and JavaScript**, designed for fast browsing, searching, and sending scripts directly to an external editor.

## Features

*  Fast script loading using ScriptBlox API
*  Real-time script search
*  Infinite scroll pagination
*  One-click copy to clipboard
*  Send scripts directly via `window.chrome.webview.postMessage`
*  Dark premium UI optimized for `#141414` background
*  Minimal, clean, and distraction-free design
*  Disabled text selection, drag, and context menu

## UI Overview

* Sticky search bar
* Card-based script layout
* Script preview image
* Script title & game name
* Copy & Send actions per script

## Integration

This ScriptHub is designed to be embedded inside apps using **WebView2**.

To receive scripts on the host side:

```js
window.chrome.webview.postMessage(script);
```

## Tech Stack

* HTML5
* CSS3 (Grid, animations, custom scrollbar)
* Vanilla JavaScript (no frameworks)

## Data Source

Scripts are fetched from:

* ScriptBlox API
* Multiple CORS proxies for reliability

## Notes

* No backend required
* Works fully offline **except** for API requests
* Keyboard shortcuts and dev tools are intentionally blocked for UI control

## License

Open-source.
Feel free to modify, improve, or integrate it into your own projects.
