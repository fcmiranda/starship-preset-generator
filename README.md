# 🚀 Starship Separator & Prompt Studio

> An interactive web-based visualizer, separator explorer, and preset generator for the [Starship](https://starship.rs) cross-shell prompt.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/Live-Demo-brightgreen.svg)](https://fcmiranda.github.io/starship-preset-generator/)

---

## ✨ Features

- **🎨 Creative Separator Presets**: Explore and experiment with various Powerline glyphs, smooth shades, angled chevrons, rounded bubbles, flame accents, waves, and hex blocks.
- **🌈 Curated Color Palettes**: Seamlessly switch between popular terminal aesthetics (Catppuccin Mocha, Tokyo Night, Dracula, Nord, Rose Pine, Gruvbox, Cyberpunk, and more).
- **⚡ Live Interactive Prompt Studio**: Real-time prompt preview reflecting your chosen directory path, git branch, execution status, and separator style.
- **📥 One-Click Export**: Copy the generated `starship.toml` directly to your clipboard or download it as a configuration file.
- **🏎️ Zero Dependencies**: 100% client-side HTML, CSS, and vanilla JavaScript. No build step or backend required.

---

## 🚀 Live Demo

Access the studio directly in your browser:
👉 **[fcmiranda.github.io/starship-preset-generator](https://fcmiranda.github.io/starship-preset-generator/)**

---

## 🛠️ Usage

### Quick Start
Open `index.html` in any modern web browser:

```bash
# Using python http server
python3 -m http.server 8080

# Or open directly
xdg-open index.html
```

### Applying your config to Starship
1. Customize your prompt design and colors in the Studio.
2. Click **Copy TOML** or **Download starship.toml**.
3. Place or append the configuration into your Starship config file:
   ```bash
   cp starship.toml ~/.config/starship.toml
   ```
4. Restart your shell or run `source ~/.zshrc` / `source ~/.bashrc`.

---

## 📄 License

MIT © [Felipe Miranda](https://github.com/fcmiranda)
