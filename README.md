# 🌐 MyBrowser — Minimal but Mighty Custom Browser

**MyBrowser** is a super simple Electron-based web browser built for one thing: **being YOUR browser**. It’s clean, compact, and fully customizable — made for devs, by a dev. Want to turn it into a private kiosk? A student-safe browser? Or just a cool app that loads your dashboard? **This is your starting point.**

---

## ✨ FEATURES

* ⚡ **Blazing fast launch**
* 🧼 **Minimal interface** — just what you need
* 🧰 **Fully editable HTML, CSS, and JS**
* 🧠 Powered by **Electron** under the hood
* 💻 Bundled into a standalone `.exe` for Windows
* 🎨 Modify anything — layout, theme, functionality — right from the source files

---

## 🗂️ FILE STRUCTURE

Inside the `resources/app/` folder:

| File                | Purpose                                          |
| ------------------- | ------------------------------------------------ |
| `index.html`        | Your homepage. This is the main content.         |
| `style.css`         | Styling — change fonts, colors, layout, etc.     |
| `main.js`           | Electron launcher logic                          |
| `renderer.js`       | Frontend browser behavior                        |
| `preload.js`        | Secure preload scripts for Electron              |
| `service-worker.js` | Add PWA features or background control           |
| `manifest.json`     | App manifest (mainly used by browser-like apps)  |
| `package.json`      | Main config — app name, version, and entry point |

All these are editable — no build steps needed to just tweak content!

---

## 💻 HOW TO CUSTOMIZE

1. **Locate the install directory** — the `MyBrowser-win32-x64/resources/app/` folder is where all the editable files live.
2. Open `index.html` and change the default content to whatever website or UI you want to load.
3. Modify `style.css` to apply your own themes.
4. Adjust behavior in `renderer.js` and `main.js`.

Make it YOURS. You can even add buttons, tabs, shortcuts, or embed other apps.

---

## 🔄 HOW TO REBUILD (Optional)

If you want to rebuild the EXE after editing:

1. Install [Node.js](https://nodejs.org/) if you haven’t already.
2. Run this in your terminal:

```bash
npm install -g electron-packager
cd path/to/project
npm install
electron-packager . MyBrowser
```

This will create a new folder like `MyBrowser-win32-x64` with a fresh `.exe` using your edits!

---

## 📦 DISTRIBUTION

You can zip the generated `.exe` folder and send it to friends, classmates, or use it as a launcher for local projects or personal dashboards. It’s THAT easy.

---

## 🔒 SECURITY NOTE

This is a minimal Electron app — no external dependencies beyond Electron itself. You can expand it with full Node.js or browser APIs, but always be mindful of the risks when loading external content.

---

## 🚀 CREDITS

Built by **MicahThePro** — dev, visionary, and absolute legend.

> Make it yours. Make it better. Make it wild.
