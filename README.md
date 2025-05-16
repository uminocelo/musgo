# Musgo CSS Framework 🌿

**Musgo is a classless, minimalistic CSS framework designed for simplicity and elegance.**

It provides sensible default styling for HTML elements, allowing you to create clean and modern-looking web pages with minimal setup and without writing custom CSS classes for basic layout and typography. Musgo embraces semantic HTML and aims to be as unobtrusive as possible.

**Goals:**

* **Classless:** No need to litter your HTML with utility classes for basic styling. Musgo styles raw HTML elements.
* **Minimalistic:** Provides essential styling without being overly opinionated or bloated.
* **Easy to Use:** Simply link the CSS file and start writing semantic HTML.
* **Customizable:** Easily themeable using CSS custom properties (variables).
* **No JavaScript:** Pure CSS for styling.

---

## Table of Contents

* [Demo](#demo)
* [Quick Start](#quick-start)
* [Features](#features)
* [Customization](#customization)
    * [Using CSS Variables](#using-css-variables)
    * [Dark Mode](#dark-mode)
* [Browser Support](#browser-support)
* [Contributing](#contributing)
* [License](#license)

---

## Demo

Check out the live demo to see Musgo in action:

➡️ **[View Demo](https://uminocelo.github.io/musgo/demo/index.html)**

---

## Quick Start

Getting started with Musgo is incredibly simple.

1.  **Download:**
    Get the latest `musgo.css` file from the `css/` directory of this repository or from the [releases page](https://github.com/uminocelo/musgo/releases).

2.  **Link in HTML:**
    Include the `musgo.css` file in the `<head>` of your HTML document:

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>My Musgo-styled Page</title>
        <link rel="stylesheet" href="css/musgo.css">
    </head>
    <body>
        <h1>Hello, Musgo!</h1>
        <p>This page is styled with Musgo CSS.</p>
    </body>
    </html>
    ```

That's it! Musgo will now apply its default styles to your HTML elements.

---

## Features

* Sensible defaults for typography (headings, paragraphs, links, lists, code blocks, blockquotes).
* Basic styling for forms (inputs, buttons, select, textarea, fieldset).
* Clean table styling.
* Responsive images and basic figure/figcaption styling.
* Support for `<details>` and `<summary>` elements.
* Dark mode support via `data-theme="dark"` attribute.
* Customization through CSS variables.
* Lightweight and fast.

---

## Customization

Musgo is designed to be easily customizable using CSS custom properties (variables).

### Using CSS Variables

You can override the default theme colors and other properties by redefining the CSS variables in your own stylesheet or directly in a `<style>` tag *after* linking `musgo.css`.

**Core Variables (see `musgo.css` for the full list):**

```css
/* Example: Creating your own light theme variant */
:root {
  --musgo-primary-color: #BF5700; /* Your brand's primary color */
  --musgo-primary-hover-color: #a34a00;
  --musgo-text-color: #333333;
  --musgo-bg-color: #fdfcfb;
  --musgo-link-color: var(--musgo-primary-color);
  /* ... and so on for other variables ... */
}
```

Place these overrides in a <style> tag in your HTML head (after Musgo's link) or in a separate CSS file linked after `musgo.css`.
For a detailed list of all available CSS variables and how to use them, please refer to the Customization Guide. 

### Dark Mode

Musgo includes a dark theme that can be activated by adding the data-theme="dark" attribute to the <body> tag or any parent container:

```html
<body data-theme="dark">
</body>
```

You can also toggle this attribute with JavaScript to allow users to switch themes. The dark theme variables are defined within the [data-theme="dark"] selector in musgo.css and can also be overridden.

### Browser Support

Musgo aims to support all modern web browsers that have good support for CSS Custom Properties.
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

Older browsers like Internet Explorer are not supported.

## Contributing

Contributions are welcome! Whether it's bug reports, feature suggestions, or pull requests, your help is appreciated.
Please read our Contributing Guidelines before submitting a pull request.

Ideas for contribution:

- Improving accessibility.
- Adding more data-* attribute styling options.
- Refining existing element styles.
- Expanding documentation.

## License
Musgo is open-source software licensed under the MIT License.