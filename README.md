Easy light weight browser
# 🌎 GEO

GEO


  ┌──────────────────────────────────────┐
  │  GEO — Lightweight Desktop Browser   │
  │  Version: 0.1.0                      │
  │  Status: In Development               │
  └──────────────────────────────────────┘

  Platform: macOS / Windows / Linux
  Engine:   Tauri 2 + Rust
  UI:       HTML / CSS / JavaScript
  RAM:      ~500 MB free recommended
```

> **CONTACT:** If you encounter any problems, please contact **[azadpelia13@gmail.com]**.
> **Geo is still in development, so bugs and unfinished features are expected.**

---

# 🌎 What is Geo?

**Geo** is a lightweight desktop web browser built around a simple idea:

> Make a browser that feels like a real desktop application while keeping the interface clean, fast, and customizable.

Geo has a frosted-glass interface, tabs, navigation controls, settings, and a command menu.

Instead of pretending to be a browser using normal HTML `<iframe>` elements, Geo creates **real browser windows** for web pages. This allows websites that normally block iframes to work normally.

---

# 💡 Why I Made Geo

I wanted to make my own browser instead of just using an existing one.

Geo is also a learning project. It combines:

* Rust
* Tauri
* JavaScript
* HTML
* CSS
* Desktop application development
* Browser concepts

The goal is to continue improving Geo over time and eventually turn it into a much more complete browser.

This project is **not finished yet**.

---

# 💻 System Requirements

Geo is designed to work on:

| Operating System | Supported |
| ---------------- | --------- |
| macOS            | ✅ Yes     |
| Windows          | ✅ Yes     |
| Linux            | ✅ Yes     |

### Memory

Geo needs approximately:

**500 MB of free RAM**

More available RAM is recommended if you plan to open multiple tabs or large websites.

### Required software

You need:

* Node.js
* Rust
* npm

You only need to install these once.

---

# 🚀 QUICK SETUP

## 1. Install Node.js

Go to:

https://nodejs.org

Download the **LTS** version.

Install it using the normal installation options.

---

## 2. Install Rust

Go to:

https://rustup.rs

Install Rust using the instructions for your operating system.

After installation, **restart your Terminal**.

---

# 📁 3. Open the Geo folder

Open Terminal / PowerShell / Command Prompt.

Go inside the `app` folder.

Example:

```bash
cd Geo-Browser-2/app
```

If you downloaded the project somewhere else, use the location of your own folder.

### Easy method

You can type:

```bash
cd
```

then drag the `app` folder into the Terminal window and press **Enter**.

---

# 📦 4. Install dependencies

Run:

```bash
npm install
```

Wait for it to finish.

This downloads the packages Geo needs.

---

# 🖼️ 5. Create the app icon

Geo needs icons before creating a finished application.

Choose any square PNG image for the Geo icon.

Then run:

```bash
npm run icon -- /path/to/your/icon.png
```

Replace:

```text
/path/to/your/icon.png
```

with the actual location of your image.

For example:

```bash
npm run icon -- ~/Downloads/geo.png
```

---

# ▶️ 6. Start Geo

Run:

```bash
npm run dev
```

The first startup can take a few minutes.

You may see a lot of text such as:

```text
Compiling...
Building...
Finished...
```

**This is normal.**

Rust has to compile the application.

When it finishes, the Geo window should open.

---

# 🏗️ BUILD GEO

If you want to create a finished application instead of running the development version, use:

```bash
npm run build
```

The finished application will be placed inside:

```text
app/src-tauri/target/release/bundle/
```

Depending on your operating system, you can get a packaged application such as:

* macOS `.app` / `.dmg`
* Windows application
* Linux package

---

# 🛠️ COMMON PROBLEMS

## `Could not read package.json`

You are probably in the wrong folder.

Make sure you are inside:

```text
Geo-Browser-2/app
```

Then run:

```bash
npm install
```

---

## `Missing script: tauri`

Don't run:

```bash
npm run tauri dev
```

Use:

```bash
npm run dev
```

---

## `failed to open icon`

Geo probably doesn't have its required icons.

Run:

```bash
npm run icon -- /path/to/your/icon.png
```

Then try:

```bash
npm run dev
```

again.

---

## Rust errors

Make sure Rust is installed:

```bash
rustc --version
```

You should see a Rust version.

Also check:

```bash
cargo --version
```

If both commands work, Rust is installed correctly.

---

# 🧭 PROJECT STRUCTURE

```text
Geo-Browser-2/
│
├── README.md
│
├── HOW-TO-RUN.txt
│
└── app/
    │
    ├── package.json
    │
    ├── src/
    │   ├── index.html
    │   │
    │   ├── css/
    │   │   ├── app.css
    │   │   └── glass.css
    │   │
    │   └── js/
    │       ├── app.js
    │       └── settings.js
    │
    └── src-tauri/
        │
        ├── Cargo.toml
        ├── build.rs
        ├── tauri.conf.json
        │
        └── src/
            └── main.rs
```

---

# ⚙️ HOW GEO WORKS

Geo is built using **Tauri 2**.

The project has two main parts.

### Frontend

The frontend controls what you see:

```text
HTML
 ↓
CSS
 ↓
JavaScript
 ↓
Geo Interface
```

This handles things like:

* Tabs
* Buttons
* Navigation
* Settings
* Glass UI
* Command menu

### Backend / Desktop Layer

Rust + Tauri turns the frontend into a real desktop application.

```text
JavaScript / HTML / CSS
          ↓
        Tauri
          ↓
         Rust
          ↓
    Desktop Window
```

Geo also uses separate browser windows for web content instead of relying on normal iframe-based fake browser tabs.

That means websites can load normally even when they prevent themselves from being embedded inside an iframe.

---

# 🔬 TECHNOLOGIES

```text
Frontend
├── HTML
├── CSS
└── JavaScript

Desktop
├── Tauri 2
└── Rust

Package Management
└── npm
```

---

# 🧪 DEVELOPMENT STATUS

```text
Geo 0.1.0

[████░░░░░░] Early Development
```

Geo is **not production-ready**.

You may encounter:

* Bugs
* Crashes
* Missing features
* UI problems
* Website compatibility issues
* Unexpected behavior

If you find something broken, please report it.

---

# 📬 CONTACT

If you encounter a problem, please contact:

**[azadpelia13@gmail.com]**

When reporting a problem, please include:

```text
Operating System:
Geo Version:
What happened:
What you expected:
Error message:
Steps to reproduce:
```

A screenshot of the error is also helpful.

---

# 🌎 THANK YOU

Thank you for taking the time to read the Geo README and try the project.

Geo is still being built, and every bug report, idea, and bit of feedback helps make it better.

**Thanks for using Geo.**

       🌎
      GEO

  Built with curiosity.
  Improved with every version.

  Thank you for reading.
```
