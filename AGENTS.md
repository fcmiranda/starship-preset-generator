# AGENTS.md — Repository Guidelines & Operating Manual

This repository contains **Starship Studio**, an interactive web-based visual editor and preset generator for the [Starship](https://starship.rs) prompt.

---

## 🤖 Rules for AI Coding Assistants (Agents)

### 1. Git & Commit Guidelines
- **Always commit in English** whenever implementing a new feature, improvement, refactoring, or bug fix requested by the user.
- Use [Conventional Commits](https://www.conventionalcommits.org/) format:
  - `feat: <description>` for new features or capabilities
  - `fix: <description>` for bug fixes or corrections
  - `style: <description>` for UI/UX tweaks or formatting
  - `docs: <description>` for documentation or SEO updates
  - `refactor: <description>` for code restructuring without changing behavior
- Make atomic, well-tested commits with descriptive messages.

### 2. Architecture & Design Principles
- **Zero Build Step & Zero External Frameworks**:
  - The project is built entirely in vanilla HTML5, CSS3, and modern client-side JavaScript.
  - Do not introduce heavy dependencies, build tools (Webpack, Vite, Tailwind CLI), or npm runtime dependencies unless explicitly instructed by the user.
- **Font & Glyph Rendering**:
  - The UI relies on Nerd Font and Powerline glyphs.
  - Always maintain high-contrast styling and proper line-height scaling for Powerline separators to prevent vertical cutoff.
- **Starship Schema Compatibility**:
  - All generated TOML configs must adhere to the official Starship configuration schema (`https://starship.rs/config-schema.json`).

### 3. SEO & Discoverability
- Maintain `<meta>` description, Open Graph, Twitter cards, and Schema.org JSON-LD structured data in `index.html`.
- Keep `robots.txt` and `sitemap.xml` in sync with any structural or URL changes.

---

## 🛠️ Testing & Local Verification
- Before finishing any task or committing changes:
  1. Validate HTML structure (e.g. `python3 -m html.parser` or unclosed tag checks).
  2. Verify JavaScript execution and syntax (e.g. `node -e "..."`).
  3. Ensure default configurations remain intact unless intentionally changed.
