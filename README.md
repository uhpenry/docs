# Uhpenry Docs Repository

Welcome to the **Uhpenry Documentation Repository**! 🚀

This repository contains the **official documentation** for the Uhpenry platform. It’s open-source and designed for **developers, contributors, and users** to explore, learn, and contribute content that helps the Uhpenry community.

---

## Table of Contents

1. [About](#about)
2. [Repository Structure](#repository-structure)
3. [Contribution Guidelines](#contribution-guidelines)
4. [Adding Images or Assets](#adding-images-or-assets)
5. [MDX & Meta Usage](#mdx--meta-usage)
6. [License](#license)
7. [Contact](#contact)

---

## About

Uhpenry is a **developer-first marketplace and trust layer**. This docs repository supports the platform by providing:

- Tutorials and getting started guides
- Feature deep dives
- Monetization, licensing, and security explanations
- API references, glossary, and FAQs

We welcome contributions from developers to **improve clarity, add examples, and keep the docs up-to-date**.

---

## Repository Structure

All documentation lives in `src/content/docs`:

```
docs/
└─ platform-guide/
   ├─ getting-started/
   │   ├─ index.mdx
   │   └─ meta.json
   ├─ projects-features/
   │   ├─ index.mdx
   │   └─ meta.json
   ├─ platform-core/
   │   ├─ index.mdx
   │   └─ meta.json
   ├─ reference/
   │   ├─ index.mdx
   │   └─ meta.json
   └─ ...
```

**Key points:**

- Each section folder contains:
  - `.mdx` files for content
  - `meta.json` for metadata (title, description, order, tags)
- Assets (images, diagrams, code snippets) go in the same folder in an `assets/` subfolder.
- Example:  
```

getting-started/assets/setup-diagram.png

````

---

## Contribution Guidelines

We welcome contributions from everyone! Please follow these steps:

1. **Fork the repository** and clone it locally.
2. **Create a branch** for your changes:
   ```bash
   git checkout -b add-feature-docs
````

3. **Add or update content** using `.mdx` files.
4. **Update `meta.json`** if adding a new page or section:

   ```json
   {
     "title": "Installation Guide",
     "description": "Step-by-step installation instructions",
     "order": 2,
     "tags": ["setup", "getting-started"]
   }
   ```
5. **Include assets** in the folder’s `assets/` subfolder.
6. **Commit & push changes**:

   ```bash
   git add .
   git commit -m "Add installation guide"
   git push origin add-feature-docs
   ```
7. **Open a Pull Request (PR)** with a clear description of your changes.

**Tips:**

* Use meaningful headings and examples in `.mdx`.
* Include code blocks for clarity:

````jsx
```js
console.log('Hello Uhpenry!');
````

````
- Keep images optimized and in PNG/JPG/WebP format.

---

## Adding Images or Assets

- Place images in the section’s `assets/` folder.
- Reference images in `.mdx` like so:
```mdx
import SetupDiagram from './assets/setup-diagram.png';

![Setup Diagram](./assets/setup-diagram.png)
````

* For multiple assets, create subfolders like `images/` or `diagrams/` inside `assets/`.

---

## MDX & Meta Usage

* **MDX files** can contain standard Markdown + React components.
* **meta.json** fields:

```json
{
  "title": "Getting Started",
  "description": "Intro guides for new Uhpenry users",
  "order": 1,
  "tags": ["onboarding", "intro"]
}
```

* The platform uses `meta.json` to dynamically build navigation and search.

---

## License

This repository is licensed under **[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)**.
You are free to **share and adapt the content**, provided you **give appropriate credit** to Uhpenry and indicate if changes were made.

---

## Contact

For questions or guidance:

* Email: [support@uhpenry.com](mailto:support@uhpenry.com)
* GitHub Issues: Use this repository’s **Issues** tab for reporting errors or proposing new docs.

---

Thank you for helping make **Uhpenry Docs** clear, accurate, and helpful!
