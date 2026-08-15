<p align="center">
  <img src="assets/Logo.png" alt="Geo logo" width="220" />
</p>

<h1 align="center">Geo</h1>

<p align="center">
  A small, fast desktop web browser with a cool frosted-glass look.
</p>

<p align="center">
  <img src="assets/1.png" alt="Screenshot of the Geo browser" width="700" />
</p>

---

## What is Geo?

Geo is a lightweight desktop web browser. It has tabs, a settings
panel, and a fun frosted-glass style. It's still being built, so
expect a few bugs here and there.

Most simple browser projects fake their tabs using something called
an `<iframe>`. The problem is that big sites like Google **block**
iframes on purpose, as a safety rule. So those fake browsers just
show an error instead of the real page.

Geo doesn't do that. Every tab in Geo is a **real, separate browser
window**, stacked right on top of the app — the same way Chrome or
Safari does it. That means real websites load the normal way and
nothing gets blocked.

## Why I made Geo

I wanted to build my own browser instead of just using one that
already exists. It's also a learning project that pulls together:

- Rust
- Tauri
- JavaScript
- HTML
- CSS
- Desktop app building
- Browser concepts

This project isn't finished yet, and I plan to keep improving it.

## What's inside this folder

```
Geo-Browser/
├── README.md          <- you are here
├── HOW-TO-RUN.txt      <- step-by-step instructions, no jargon
├── assets/              images used in this README
│   ├── Logo.png
│   └── 1.png
└── app/                 the actual app code
    ├── package.json      tells npm how to start/build the app
    ├── src/                everything you SEE (the UI)
    │   ├── index.html      the page layout: sidebar, tabs, toolbar
    │   ├── css/             colors, spacing, the glass look
    │   │   ├── glass.css     the color/design rules
    │   │   └── app.css       everything else (layout, buttons, etc.)
    │   └── js/               the logic that makes buttons do things
    │       ├── app.js         tabs, navigation, the ⌘K menu
    │       └── settings.js    the settings screen
    └── src-tauri/           the Rust part that makes it a real
                              desktop app, not just a webpage
        ├── src/main.rs        creates each tab as its own real window
        ├── Cargo.toml         Rust's version of package.json
        ├── build.rs           a small setup script Rust runs first
        └── tauri.conf.json    app name, window size, icon settings
```

## Before you run it

You need two free programs installed first:

1. **Node.js** — https://nodejs.org (pick the LTS version)
2. **Rust** — https://rustup.rs

You only need to do this once. After that, check **HOW-TO-RUN.txt**
for the exact steps to start the app.

## Good to know

- The first time you run Geo, your computer has to download and
  build a bunch of Rust code. That can take a few minutes — it's
  normal, not stuck.
- If it complains about a missing icon, that just means the app icon
  files haven't been generated yet. HOW-TO-RUN.txt covers that too.

## System requirements

| Operating System | Supported |
| ----------------- | --------- |
| macOS              | ✅ Yes     |
| Windows            | ✅ Yes     |
| Linux              | ✅ Yes     |

About 500 MB of free RAM is recommended.

## Status

Geo is early in development. You may run into bugs, crashes, or
missing features. If you find something broken, feel free to reach
out — feedback helps make it better.

**Thanks for checking out Geo.**
