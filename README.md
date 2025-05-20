<p align="center">
  <img src="https://img.shields.io/badge/demo-live-brightgreen?style=for-the-badge&logo=github" alt="Musgo Demo Badge">
  <img src="https://img.shields.io/github/license/uminocelo/musgo?style=for-the-badge" alt="License MIT">
</p>

<h1 align="center">🌿 Musgo</h1>
<p align="center">A classless, block-based CSS framework for clean, responsive, semantic HTML.</p>

---

## ✨ Features

- ✅ **Classless styling** — beautiful defaults out-of-the-box
- ✅ **Custom grid system** using semantic `data-musgo-block` attributes
- ✅ **Responsive design** with mobile-first breakpoints
- ✅ **Dark mode** support with `data-theme="dark"`
- ✅ **Accessible form elements** and validation states
- ✅ **Built with SCSS** for maintainability and modularity

---

## 🔗 Live Demo

Explore the framework live:

👉 **[https://uminocelo.github.io/musgo](https://uminocelo.github.io/musgo)**

You’ll find a full-featured grid demo and usage examples.

---

## 📦 Installation

Clone the repo and include the CSS files:

```html
<link rel="stylesheet" href="css/musgo.css">
<link rel="stylesheet" href="css/musgo-block-grid.css">
```

Or download the latest release from the [Releases page](https://github.com/uminocelo/musgo/releases).

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
Use data-musgo-block-sm, -md, -lg, -xl for responsive control.

## 🛠️ Project Structure

```bash
musgo/
├── css/
│   ├── musgo.css                # Classless styling
│   ├── musgo-block-grid.css     # Grid layout system
│   └── scss/                    # Source SCSS files
├── demo/
│   └── index.html               # Full Musgo demo
├── docs/
│   └── USAGE.md                 # Detailed usage documentation
├── README.md
└── LICENSE
```

## 🧱 Grid System

Musgo uses a 12-column grid with predefined block sizes:

| Block | Columns | Percentage   | 
|-------|---------|--------------| 
| 1	    | 1	      |   ~8.33%     | 
| 2	    | 3       |   25%        | 
| 3	    | 6	      |   50%        | 
| 4	    | 9	      |   75%        | 
| 5	    | 12      |   100%       | 

You can combine blocks and adjust responsiveness with `data-musgo-block-[breakpoint]``.

## 🌗 Dark Mode

Enable dark mode by setting the data-theme="dark" attribute on the <html> or <body> element:

```html
<html data-theme="dark">
```

All colors and backgrounds will adapt automatically using CSS custom properties.

## 📄 License

Licensed under the MIT License.

## 🧑‍💻 Author

Built with ❤️ by [uminocelo](https://github.com/uminocelo).

📖 [Full Usage Guide →](docs/USAGE.md)