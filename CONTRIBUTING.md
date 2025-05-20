# 🤝 Contributing to Musgo

Thank you for your interest in contributing to **Musgo**, a classless, block-based CSS framework! Whether you're fixing bugs, improving documentation, or suggesting new features — you're very welcome here.

---

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Reporting Bugs](#reporting-bugs)
- [Suggesting Features](#suggesting-features)
- [Development Guide](#development-guide)
- [Pull Request Process](#pull-request-process)

---

## 🧠 Code of Conduct

This project follows a [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/).  
Be respectful, inclusive, and constructive in your communication.

---

## 🚀 Getting Started

### 1. Fork the Repository

Click the **Fork** button on GitHub and clone your fork locally:

```bash
git clone https://github.com/uminocelo/musgo.git
cd musgo
```

### 2. Install Dev Dependencies

```bash
npm install
```

### 3. Build the CSS

```bash
npm run build
```


## 🐞 Reporting Bugs

Please open a bug report and include:

- Expected vs actual behavior
- Steps to reproduce
- HTML/CSS snippet or link to a demo
- Browser(s) and environment info


## 💡 Suggesting Features

We love improvement ideas! Please use the [feature request form](https://github.com/uminocelo/musgo/issues/new?template=feature_request.yml) and tell us:

- What you'd like to see
- Why it's useful
- Any alternatives you’ve considered


## 🛠 Development Guide

Project Structure:

```bash
css/
├── musgo.css                # Compiled classless styling
├── musgo-block-grid.css     # Compiled layout system
└── scss/                    # SCSS source files
demo/                        # HTML demos
docs/                        # Documentation
```

## SCSS Compilation

```bash
npm run build
```

- `musgo.scss` → `musgo.css`
- `musgo-block-grid.scss` → `musgo-block-grid.css`


## ✅ Pull Request Process
1. Fork → Branch → Commit
2. Run `npm run build` and test the output
3. Follow coding conventions:
  - Use SCSS variables and maps
  - Keep things modular
4. Document new features or changes
5. Submit your pull request

We'll review as soon as possible and leave feedback or merge 🚀


## 🧑‍💻 Maintainers

- [uminocelo](https://github.com/uminocelo)