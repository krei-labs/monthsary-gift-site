<p align="center">
  <img src="./readme-banner.png" alt="1st Monthsary Gift Website banner" width="600">
</p>

<h1 align="center">1st Monthsary Gift Website 💌</h1>

<p align="center">
  A romantic, interactive static website template for celebrating a monthsary or anniversary — content-driven, no backend required.
</p>

<p align="center">
  <a href="https://monthsary-gift-site.netlify.app/"><img alt="Live Demo" src="https://img.shields.io/badge/Live%20Demo-View%20Site-ff4d8d?logo=netlify&logoColor=white"></a>
  <img alt="HTML" src="https://img.shields.io/badge/HTML5-Static%20Site-e34c26?logo=html5&logoColor=white">
  <img alt="CSS" src="https://img.shields.io/badge/CSS3-Animations-1572B6?logo=css3&logoColor=white">
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-Vanilla-f7df1e?logo=javascript&logoColor=black">
  <img alt="Netlify" src="https://img.shields.io/badge/Deploy-Netlify-00c7b7?logo=netlify&logoColor=white">
  <img alt="License" src="https://img.shields.io/badge/License-Personal%20Use-lightgrey">
</p>

<p align="center">
  <strong>🔗 Live Demo:</strong> <a href="https://monthsary-gift-site.netlify.app/">monthsary-gift-site.netlify.app</a>
</p>

---

> **🔑 Demo password:** the live demo is gated behind a simple client-side password screen. Enter **`051626`** to unlock it. This is a personal-gift template, not real security — see the `SITE_PASSWORD` comment in `index.html` if you want to set your own.

---

> **Privacy note:** This is the public, GitHub-safe version of a commissioned personal gift site. All real photos, songs, names, and dates from the original delivery have been removed or replaced with generic placeholders — see [Privacy & Content](#-privacy--content) below. Everything shown here is a reusable template, not the original recipient's content.

---

## 📑 Table of Contents

- [Features](#-features)
- [Project Structure](#-project-structure)
- [Customize Your Content](#-customize-your-content)
- [Adding Your Own Media](#-adding-your-own-media)
- [Logo & Favicon](#-logo--favicon)
- [Password Protection](#-password-protection)
- [Run Locally](#-run-locally)
- [Deploy to Netlify](#-deploy-to-netlify)
- [Privacy & Content](#-privacy--content)
- [License](#-license)
- [Author](#-author)

---

## ✨ Features

- 💌 Romantic multi-step scrolling experience
- 📝 Love-letter section, editable from a single content file
- 💭 Reasons + memory-highlight sections
- 📅 First-month timeline
- 🎉 Celebration section with a **Top 5 song picker**, each paired with a short poem
- 🎧 Built-in audio player
- 🎊 Confetti, heart rain, and extra emotion effects (via `canvas-confetti` and `GSAP`)
- ⏳ Countdown badge for your monthsary date
- 🗂️ Content managed entirely from a JSON file — no database, no backend

---

## 📂 Project Structure

```text
monthsary-gift-site-main/
├── index.html               # Main page markup, layout, and script includes
├── favicon.png              # Glowing heart favicon matching the site's pink/purple theme
├── readme-banner.png        # Banner used at the top of this README
├── data/
│   └── content.json         # All editable text, timeline, songs, and photo paths
├── netlify.toml              # Netlify deployment config
├── LICENSE.md                # KREI-LABS license
└── README.md                 # Project documentation
```

---

## ✍️ Customize Your Content

Everything user-facing lives in `data/content.json`. You can edit:

- Hero title and intro
- Love-letter text
- Timeline entries and milestone dates
- Reasons and memory captions
- Top 5 songs (name, artist, file path, poem)
- Memory photo paths

No code changes are needed for a full re-personalization — just edit the JSON.

---

## 🖼️ Adding Your Own Media

### Music
Place your files inside `media/music/`:
```
song1.mp3
song2.mp3
song3.mp3
song4.mp3
song5.mp3
```

### Photos
Place your files inside `media/photos/`:
```
memory1.jpg ... memory12.jpg
```

If a memory photo is missing, the page falls back to `./media/photos/placeholder.jpg` — add your own placeholder image if you'd like a graceful fallback.

---

## 🐱 Logo & Favicon

`favicon.png` and `readme-banner.png` are a generated glowing heart badge built from the site's own CSS palette (`--bg`, `--pink`, `--rose`, `--text` in `index.html`), so it matches the page's dark purple/pink glass aesthetic.

- The favicon is linked in `index.html`: `<link rel="icon" type="image/png" href="./favicon.png" />`
- To use your own logo, just replace `favicon.png` with any square image (128×128 or larger).

---

## 🔒 Password Protection

The site shows a password screen (`#passwordModal`) before revealing the content. The password is set in plain text in `index.html`:

```js
// ⚠️ SITE PASSWORD: change '051626' below to set your own unlock password (this is the entry gate the visitor must type in)
const SITE_PASSWORD='051626', BG_MUSIC_SRC='./media/music/background.mp3';
```

Search for `SITE_PASSWORD` in `index.html` to find and change it. Keep in mind this only lives in client-side JavaScript — anyone who views the page source can read it, so treat it as a fun gate for your recipient, not real security.

---

## ▶️ Run Locally

Because the page fetches `content.json`, it needs to be served from a local server rather than opened directly as a file.

**Option 1 — VS Code Live Server**
Install the Live Server extension, then right-click `index.html` → *Open with Live Server*.

**Option 2 — Python**
```bash
python -m http.server 5500
```
Then open `http://localhost:5500`.

---

## 🚀 Deploy to Netlify

1. Push this folder to GitHub (optional but recommended).
2. On Netlify, choose **Add new site** → import the project (or drag-and-drop the folder).
3. Set the publish directory to `.`
4. Deploy — `netlify.toml` is already included.

---

## 🔐 Privacy & Content

This repository is the **sanitized, shareable version** of a commissioned personal project. Before publishing:

- All original photos and songs were **removed** from the public repository for privacy.
- Names were replaced with generic placeholders (`My Love` / `[Your Name]`).
- The specific monthsary date was replaced with `[Your Monthsary Date]`.
- The personal love-letter and surprise-message text were rewritten into generic, reusable versions.

If you're using this as a template for your own gift site, replace the placeholders in `data/content.json` with your own words, photos, and songs.

---

## 📄 License

Personal/portfolio project. Feel free to use this as a learning reference or starting template; if you plan to redistribute or resell it, please contact the author first.

---

## 👤 Author

**Christian G. Maranan**
Computer Engineering Student — Major in Machine Learning
at Tanauan City College

- **GitHub:** [@krei-labs](https://github.com/krei-labs)
- **Instagram:** [@krei_in](https://instagram.com/krei_in)
- **Email:** [christianmaranan0303@gmail.com](mailto:christianmaranan0303@gmail.com)

---

<p align="center"><strong>Build. Learn. Experiment.</strong> — kréi / Krei Labs</p>
