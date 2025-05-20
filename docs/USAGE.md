# 🧰 Musgo CSS — Usage Guide

Welcome to **Musgo**, a classless CSS framework designed for clarity, accessibility, and semantic HTML. This guide covers installation, layout principles, grid usage, and component behaviors.

---

## 📦 Installation

### CDN (Coming soon)
_(If you publish to jsDelivr or UNPKG, document that here)_

### Local

Download or clone this repository:

```bash
git clone https://github.com/uminocelo/musgo.git
```

Link the compiled CSS files in your HTML:

```html
<link rel="stylesheet" href="css/musgo.css">
<link rel="stylesheet" href="css/musgo-block-grid.css">
```

## 🧱 Grid Layout
Musgo uses a block-based responsive grid built with Flexbox.

### ✅ Block Mapping

| `data-musgo-block` | Grid Columns | Width (%)                     |
| ------------------ | ------------ | ----------------------------- |
| `"1"`              | 1            | \~8.33%                       |
| `"2"`              | 3            | 25%                           |
| `"3"`              | 6            | 50%                           |
| `"4"`              | 9            | 75%                           |
| `"5"`              | 12           | 100%                          |
| `""` (empty)       | auto         | remaining space (`flex-grow`) |

### 🧩 Basic Usage

```html
<div data-musgo-container>
  <div data-musgo-row>
    <div data-musgo-block="2">3 columns</div>
    <div data-musgo-block="3">6 columns</div>
    <div data-musgo-block="2">3 columns</div>
  </div>
</div>
```

### 🖥 Responsive Blocks

Use data-musgo-block-[breakpoint] for mobile-first control:

```html
<div data-musgo-block="5" data-musgo-block-md="3">
  Full width on small, 25% on md+
</div>
```

Supported breakpoints:

| Suffix | Min Width |
| ------ | --------- |
| `-sm`  | 576px     |
| `-md`  | 768px     |
| `-lg`  | 992px     |
| `-xl`  | 1200px    |

## 🧭 Layout Utilities

### Containers

`data-musgo-container`: centers and applies max-width
`data-musgo-container="fluid"`: full width always

### Rows

`data-musgo-row`: flex row container
`data-musgo-gutters="none"`: removes padding and negative margins

## 🎯 Alignment Utilities

### Row Alignment

```html
<div data-musgo-row data-musgo-align-items="center" data-musgo-justify-content="between">
```

Available values:

`align-items`: `start`, `center`, `end`, `stretch`, `baseline`
`justify-content`: `start`, `center`, `end`, `between`, `around`

### Self Alignment

```html
<div data-musgo-align-self="end">
```

Available values: same as `align-items`.

## ↔️ Offset & Order

```html
<div data-musgo-offset="1">Offset by 3 columns</div>
<div data-musgo-order="first">Appears first</div>
<div data-musgo-order="last">Appears last</div>
```

Breakpoints also supported: `data-musgo-offset-sm="1"`.

## 🌈 Theming & Color

Musgo uses CSS custom properties (variables) for theme control.

### Dark Mode

Activate via attribute:

```html
<html data-theme="dark">
```

All components and colors adjust automatically.

## 📝 Typography

Musgo styles headings, paragraphs, lists, blockquotes, and inline elements with consistent spacing and rhythm.

```html

<h1>Heading</h1>
<p>Paragraph with <strong>strong</strong> and <em>emphasis</em>.</p>
<blockquote>Blockquote text.</blockquote>
<code>Inline code</code>

```

## 🧾 Forms
Fully styled forms with accessibility states:

```html

<label for="email">Email</label>
<input type="email" id="email" placeholder="you@example.com">

<button type="submit">Submit</button>
<button type="button" data-variant="outline">Cancel</button>

```

Validation:

```html
<input type="email" aria-invalid="true">
```

Size:

```html
<input data-size="small">
<button data-size="large">Big Button</button>
```

## 📊 Tables

```html
<table>
  <thead>
    <tr><th>Name</th><th>Email</th></tr>
  </thead>
  <tbody>
    <tr><td>Alice</td><td>alice@example.com</td></tr>
  </tbody>
</table>
```

## 🖨 Print Support

Musgo includes a print stylesheet to ensure documents look clean and readable on paper:

- No colors or shadows
- No navigation/sidebar elements
- URLs appended to links

## 🤝 Contributing

Feel free to open issues, suggest improvements, or fork the project.