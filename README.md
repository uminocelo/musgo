<p align="center">
  <a href="https://uminocelo.github.io/musgo">
    <img src="https://img.shields.io/badge/demo-live-brightgreen?style=for-the-badge&logo=github" alt="Live Demo">
  </a>
  <a href="https://github.com/uminocelo/musgo/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/uminocelo/musgo?style=for-the-badge" alt="License">
  </a>
  <a href="https://github.com/uminocelo/musgo/actions/workflows/build.yml">
    <img src="https://github.com/uminocelo/musgo/actions/workflows/build.yml/badge.svg" alt="Build Status">
  </a>
</p>

<h1 align="center">🌿 Musgo</h1>
<p align="center">A classless, block-based CSS framework for clean, responsive, and semantic HTML — with dark mode support, accessible defaults, and zero class bloat.</p>

---

## ✨ Features

- ✅ **Classless styling** — Just write semantic HTML
- ✅ **Block-based grid** — Use simple `data-musgo-block` attributes
- ✅ **Responsive layout** — With mobile-first breakpoints (`sm`, `md`, `lg`, `xl`)
- ✅ **Dark mode** — Enabled via `data-theme="dark"`
- ✅ **Accessible forms** — With focus, disabled, and validation states
- ✅ **Modular SCSS** — Built for maintainability and easy customization

---

## 🔗 Live Demo

🧪 Try Musgo in action:  
👉 [**https://uminocelo.github.io/musgo**](https://uminocelo.github.io/musgo)

Explore the full grid system, responsive behavior, and dark mode in the demo page.

---

## 📦 Installation

### 1. Clone the repo or download it

```bash
git clone https://github.com/uminocelo/musgo.git
```

### 2. Link the compiled CSS in your HTML

```html
<link rel="stylesheet" href="css/musgo.css">
<link rel="stylesheet" href="css/musgo-block-grid.css">
```

Or download the latest release from the [Releases page](https://github.com/uminocelo/musgo/releases).

---

## 🚀 Quick Start Example

```html
<div data-musgo-container>
  <div data-musgo-row>
    <div data-musgo-block="2">3 columns</div>
    <div data-musgo-block="3">6 columns</div>
    <div data-musgo-block="2">3 columns</div>
  </div>
</div>
```

Use responsive modifiers like `data-musgo-block-sm`, `-md`, `-lg`, and `-xl` to control layout at different breakpoints.

## 🧱 Grid System

Musgo uses a 12-column grid with predefined block sizes:

| Block | Columns | Percentage   | 
|-------|---------|--------------| 
| 1	    | 1	      |   ~8.33%     | 
| 2	    | 3       |   25%        | 
| 3	    | 6	      |   50%        | 
| 4	    | 9	      |   75%        | 
| 5	    | 12      |   100%       | 

You can combine blocks and adjust responsiveness with `data-musgo-block-[breakpoint]`.

## 🌗 Dark Mode

Enable dark mode by setting the data-theme="dark" attribute on the <html> or <body> element:

```html
<html data-theme="dark">
```

Musgo automatically adjusts colors, backgrounds, and form styles using CSS variables.

## 🛠️ Project Structure

```bash
musgo/
├── css/
│   ├── musgo.css                # Classless core styles
│   ├── musgo-block-grid.css     # Grid layout engine
│   └── scss/                    # Source SCSS files (modular)
├── demo/
│   └── index.html               # Full demo page
├── docs/
│   └── USAGE.md                 # In-depth usage guide
├── README.md
└── LICENSE
```

---

## 📖 Documentation

[📘 Full Usage Guide](docs/USAGE.md)

[🧾 Code of Conduct](CODE_OF_CONDUCT.md)

[🔐 Security Policy](SECURITY.md)

## 📄 License

Licensed under the MIT License.

## 🧑‍💻 Author

Built with ❤️ by [uminocelo](https://github.com/uminocelo).