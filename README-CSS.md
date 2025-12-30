# Mastors-Gridder

**Comprehensive CSS Grid Utility Library** - Professional-grade grid classes for modern web layouts.

A powerful, flexible, and production-ready CSS utility library that provides everything you need to build responsive, complex layouts with ease. No build tools required—just pure CSS classes ready to use.

---

<p align="center">
  <a href="/">
    <img src="https://img.shields.io/badge/SASS-DOCUMENTATION-cc6699?style=for-the-badge&logo=sass&logoColor=white">
  </a>
  &nbsp;
  <a href="https://kehem-it.github.io/Mastors-Gridder/">
    <img src="https://img.shields.io/badge/FULL-DOCUMENTATION-2ea44f?style=for-the-badge&logo=readthedocs&logoColor=white">
  </a>
</p>

---

## 📋 Table of Contents

- [Installation](#-installation)
- [Quick Start](#-quick-start)
- [Grid Classes Overview](#-grid-classes-overview)
- [Quick Reference Table](#-quick-reference-table)
- [Detailed Documentation](#-detailed-documentation)
  - [Responsive Grid Classes](#responsive-grid-classes)
  - [Fixed Grid Classes](#fixed-grid-classes)
  - [Layout Pattern Classes](#layout-pattern-classes)
  - [Grid Item Classes](#grid-item-classes)
  - [Alignment & Utility Classes](#alignment--utility-classes)
  - [Responsive Modifiers](#responsive-modifiers)
- [Usage Examples](#-usage-examples)
- [Best Practices](#-best-practices)
- [Browser Support](#-browser-support)
- [FAQ](#-faq)
- [Changelog](#-changelog)

---

## 🚀 Installation

### Via CDN (Recommended for Quick Start)

Add this link in your HTML `<head>`:

```html
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/gh/KEHEM-IT/Mastors-Gridder@main/mastors-gridder.css"
/>
```

### Via NPM

Install the package:

```bash
npm i mastors-gridder
```

Then import in your CSS or HTML:

```css
@import "mastors-gridder";
```

Or link in HTML:

```html
<link
  rel="stylesheet"
  href="node_modules/mastors-gridder/mastors-gridder.css"
/>
```

### Manual Installation

Download `mastors-gridder.css` and link it in your HTML:

```html
<link rel="stylesheet" href="path/to/mastors-gridder.css" />
```

---

## ⚡ Quick Start

```html
<!-- Auto-fit responsive grid -->
<div class="grid-auto gap-lg">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>

<!-- Fixed 4-column grid -->
<div class="grid-cols-4 gap-md">
  <div>Column 1</div>
  <div>Column 2</div>
  <div>Column 3</div>
  <div>Column 4</div>
</div>

<!-- Sidebar layout -->
<div class="grid-sidebar gap-lg">
  <aside>Sidebar</aside>
  <main>Main Content</main>
</div>

<!-- Centered content -->
<div class="grid-center" style="min-height: 400px;">
  <h1>Centered Content</h1>
</div>

<!-- Span multiple columns -->
<div class="grid-cols-4">
  <div class="col-span-2">Spans 2 columns</div>
  <div>Normal</div>
  <div>Normal</div>
</div>
```

---

## 🎯 Grid Classes Overview

| Category       | Classes                                              | Use Case               |
| -------------- | ---------------------------------------------------- | ---------------------- |
| **Responsive** | `grid-auto`, `grid-fill`, `grid-cards`               | Auto-responsive grids  |
| **Fixed**      | `grid-cols-*`, `grid-rows-*`                         | Fixed column/row grids |
| **Layouts**    | `grid-sidebar`, `grid-holy-grail`, `grid-full-bleed` | Common layout patterns |
| **Items**      | `col-span-*`, `row-span-*`, `order-*`                | Grid item positioning  |
| **Alignment**  | `grid-center`, `items-*`, `self-*`                   | Content alignment      |
| **Spacing**    | `gap-*`, `gap-x-*`, `gap-y-*`                        | Grid spacing           |
| **Responsive** | `sm:*`, `md:*`, `lg:*`                               | Breakpoint modifiers   |

---

## 📊 Quick Reference Table

Complete list of all utility classes with descriptions and usage examples.

### Responsive Grid Classes

| Class            | Description                        | Usage Example                    |
| ---------------- | ---------------------------------- | -------------------------------- |
| `grid-auto`      | Auto-fit grid, min 250px columns   | `<div class="grid-auto gap-lg">` |
| `grid-auto-sm`   | Auto-fit grid, min 150px columns   | `<div class="grid-auto-sm">`     |
| `grid-auto-md`   | Auto-fit grid, min 250px columns   | `<div class="grid-auto-md">`     |
| `grid-auto-lg`   | Auto-fit grid, min 350px columns   | `<div class="grid-auto-lg">`     |
| `grid-fill`      | Auto-fill grid, keeps empty tracks | `<div class="grid-fill gap-md">` |
| `grid-fill-sm`   | Auto-fill grid, min 150px          | `<div class="grid-fill-sm">`     |
| `grid-fill-lg`   | Auto-fill grid, min 350px          | `<div class="grid-fill-lg">`     |
| `grid-cards`     | Responsive card grid, 280px min    | `<div class="grid-cards">`       |
| `grid-cards-sm`  | Card grid, 200px min               | `<div class="grid-cards-sm">`    |
| `grid-cards-lg`  | Card grid, 350px min               | `<div class="grid-cards-lg">`    |
| `grid-dense`     | Dense packing, fills gaps          | `<div class="grid-dense">`       |
| `grid-stacked`   | Mobile stack → 2 cols at 640px     | `<div class="grid-stacked">`     |
| `grid-stacked-3` | Mobile stack → 3 cols at 768px     | `<div class="grid-stacked-3">`   |

### Fixed Grid Classes

| Class          | Description         | Usage Example                |
| -------------- | ------------------- | ---------------------------- |
| `grid-cols-1`  | 1 column grid       | `<div class="grid-cols-1">`  |
| `grid-cols-2`  | 2 column grid       | `<div class="grid-cols-2">`  |
| `grid-cols-3`  | 3 column grid       | `<div class="grid-cols-3">`  |
| `grid-cols-4`  | 4 column grid       | `<div class="grid-cols-4">`  |
| `grid-cols-5`  | 5 column grid       | `<div class="grid-cols-5">`  |
| `grid-cols-6`  | 6 column grid       | `<div class="grid-cols-6">`  |
| `grid-cols-8`  | 8 column grid       | `<div class="grid-cols-8">`  |
| `grid-cols-12` | 12 column grid      | `<div class="grid-cols-12">` |
| `grid-rows-2`  | 2 equal-height rows | `<div class="grid-rows-2">`  |
| `grid-rows-3`  | 3 equal-height rows | `<div class="grid-rows-3">`  |
| `grid-rows-4`  | 4 equal-height rows | `<div class="grid-rows-4">`  |
| `grid-rows-5`  | 5 equal-height rows | `<div class="grid-rows-5">`  |

### Layout Pattern Classes

| Class                     | Description                        | Usage Example                           |
| ------------------------- | ---------------------------------- | --------------------------------------- |
| `grid-sidebar`            | Sidebar (300px) + content          | `<div class="grid-sidebar">`            |
| `grid-sidebar-sm`         | Sidebar (200px) + content          | `<div class="grid-sidebar-sm">`         |
| `grid-sidebar-lg`         | Sidebar (400px) + content          | `<div class="grid-sidebar-lg">`         |
| `grid-sidebar-right`      | Content + sidebar (300px) on right | `<div class="grid-sidebar-right">`      |
| `grid-sidebar-responsive` | Responsive sidebar (stacks mobile) | `<div class="grid-sidebar-responsive">` |
| `grid-holy-grail`         | Header/sidebars/content/footer     | `<div class="grid-holy-grail">`         |
| `grid-full-bleed`         | Content with full-width breakouts  | `<div class="grid-full-bleed">`         |
| `grid-asymmetric`         | 2:1 ratio two-column               | `<div class="grid-asymmetric">`         |
| `grid-asymmetric-reverse` | 1:2 ratio two-column               | `<div class="grid-asymmetric-reverse">` |
| `grid-masonry`            | 3-column masonry layout            | `<div class="grid-masonry">`            |
| `grid-masonry-4`          | 4-column masonry layout            | `<div class="grid-masonry-4">`          |
| `grid-equal-rows`         | Equal-height auto rows             | `<div class="grid-equal-rows">`         |

### Grid Item Classes

| Class           | Description               | Usage Example                 |
| --------------- | ------------------------- | ----------------------------- |
| `col-span-1`    | Span 1 column             | `<div class="col-span-1">`    |
| `col-span-2`    | Span 2 columns            | `<div class="col-span-2">`    |
| `col-span-3`    | Span 3 columns            | `<div class="col-span-3">`    |
| `col-span-4`    | Span 4 columns            | `<div class="col-span-4">`    |
| `col-span-5`    | Span 5 columns            | `<div class="col-span-5">`    |
| `col-span-6`    | Span 6 columns            | `<div class="col-span-6">`    |
| `col-span-full` | Span all columns (1 / -1) | `<div class="col-span-full">` |
| `row-span-1`    | Span 1 row                | `<div class="row-span-1">`    |
| `row-span-2`    | Span 2 rows               | `<div class="row-span-2">`    |
| `row-span-3`    | Span 3 rows               | `<div class="row-span-3">`    |
| `row-span-4`    | Span 4 rows               | `<div class="row-span-4">`    |
| `row-span-full` | Span all rows (1 / -1)    | `<div class="row-span-full">` |
| `order-first`   | Display first (order: -1) | `<div class="order-first">`   |
| `order-last`    | Display last (order: 999) | `<div class="order-last">`    |
| `order-1`       | Order: 1                  | `<div class="order-1">`       |
| `order-2`       | Order: 2                  | `<div class="order-2">`       |
| `order-3`       | Order: 3                  | `<div class="order-3">`       |

### Gap/Spacing Classes

| Class      | Description           | Usage Example                      |
| ---------- | --------------------- | ---------------------------------- |
| `gap-0`    | No gap                | `<div class="grid-auto gap-0">`    |
| `gap-xs`   | 0.5rem gap            | `<div class="grid-auto gap-xs">`   |
| `gap-sm`   | 1rem gap              | `<div class="grid-auto gap-sm">`   |
| `gap-md`   | 1.5rem gap            | `<div class="grid-auto gap-md">`   |
| `gap-lg`   | 2rem gap              | `<div class="grid-auto gap-lg">`   |
| `gap-xl`   | 3rem gap              | `<div class="grid-auto gap-xl">`   |
| `gap-x-sm` | 1rem horizontal gap   | `<div class="grid-auto gap-x-sm">` |
| `gap-y-sm` | 1rem vertical gap     | `<div class="grid-auto gap-y-sm">` |
| `gap-x-md` | 1.5rem horizontal gap | `<div class="grid-auto gap-x-md">` |
| `gap-y-md` | 1.5rem vertical gap   | `<div class="grid-auto gap-y-md">` |
| `gap-x-lg` | 2rem horizontal gap   | `<div class="grid-auto gap-x-lg">` |
| `gap-y-lg` | 2rem vertical gap     | `<div class="grid-auto gap-y-lg">` |

### Alignment Classes

| Class                   | Description                | Usage Example                                   |
| ----------------------- | -------------------------- | ----------------------------------------------- |
| `grid-center`           | Center items both axes     | `<div class="grid-center">`                     |
| `items-start`           | Align items to start       | `<div class="grid-auto items-start">`           |
| `items-center`          | Align items to center      | `<div class="grid-auto items-center">`          |
| `items-end`             | Align items to end         | `<div class="grid-auto items-end">`             |
| `items-stretch`         | Stretch items              | `<div class="grid-auto items-stretch">`         |
| `justify-items-start`   | Justify items to start     | `<div class="grid-auto justify-items-start">`   |
| `justify-items-center`  | Justify items to center    | `<div class="grid-auto justify-items-center">`  |
| `justify-items-end`     | Justify items to end       | `<div class="grid-auto justify-items-end">`     |
| `justify-items-stretch` | Stretch items horizontally | `<div class="grid-auto justify-items-stretch">` |
| `self-start`            | Align self to start        | `<div class="self-start">`                      |
| `self-center`           | Align self to center       | `<div class="self-center">`                     |
| `self-end`              | Align self to end          | `<div class="self-end">`                        |
| `self-stretch`          | Stretch self               | `<div class="self-stretch">`                    |
| `justify-self-start`    | Justify self to start      | `<div class="justify-self-start">`              |
| `justify-self-center`   | Justify self to center     | `<div class="justify-self-center">`             |
| `justify-self-end`      | Justify self to end        | `<div class="justify-self-end">`                |

### Responsive Modifiers

| Prefix | Breakpoint | Usage Example                              |
| ------ | ---------- | ------------------------------------------ |
| `sm:`  | 640px+     | `<div class="grid-cols-1 sm:grid-cols-2">` |
| `md:`  | 768px+     | `<div class="grid-cols-1 md:grid-cols-3">` |
| `lg:`  | 1024px+    | `<div class="grid-cols-1 lg:grid-cols-4">` |

**Available responsive classes:**

- `sm:grid-cols-2`, `sm:grid-cols-3`, `sm:grid-cols-4`
- `md:grid-cols-2`, `md:grid-cols-3`, `md:grid-cols-4`, `md:grid-cols-6`
- `lg:grid-cols-3`, `lg:grid-cols-4`, `lg:grid-cols-5`, `lg:grid-cols-6`
- `sm:col-span-2`, `sm:col-span-3`
- `md:col-span-2`, `md:col-span-3`, `md:col-span-4`

### Subgrid Classes

| Class          | Description                | Usage Example                |
| -------------- | -------------------------- | ---------------------------- |
| `subgrid-cols` | Inherit parent column grid | `<div class="subgrid-cols">` |
| `subgrid-rows` | Inherit parent row grid    | `<div class="subgrid-rows">` |
| `subgrid-both` | Inherit both axes          | `<div class="subgrid-both">` |

---

## 📖 Detailed Documentation

### Responsive Grid Classes

#### `.grid-auto` / `.grid-auto-sm` / `.grid-auto-md` / `.grid-auto-lg`

Creates a **responsive grid** that automatically fits as many columns as possible based on minimum width.

**Variants:**

- `.grid-auto-sm`: 150px minimum
- `.grid-auto-md`: 250px minimum (default)
- `.grid-auto-lg`: 350px minimum

**Use case:** Image galleries, product cards, any content that should flow naturally

```html
<div class="grid-auto gap-lg">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>
```

---

#### `.grid-fill` / `.grid-fill-sm` / `.grid-fill-lg`

Similar to `.grid-auto`, but uses `auto-fill` instead of `auto-fit`. Creates **empty columns** if there's extra space.

**Difference from `.grid-auto`:**

- `auto-fit`: Collapses empty tracks, items stretch to fill space
- `auto-fill`: Keeps empty tracks, items maintain consistent size

```html
<div class="grid-fill gap-md">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

---

#### `.grid-cards` / `.grid-cards-sm` / `.grid-cards-lg`

Responsive card grid with **min/max constraints** for better control.

**Variants:**

- `.grid-cards-sm`: 200px minimum
- `.grid-cards`: 280px minimum (default)
- `.grid-cards-lg`: 350px minimum

```html
<div class="grid-cards">
  <div class="card">Card 1</div>
  <div class="card">Card 2</div>
  <div class="card">Card 3</div>
</div>
```

---

#### `.grid-dense`

Fills gaps by placing items **densely** (useful for varying item sizes).

```html
<div class="grid-dense gap-md">
  <div class="col-span-2">Large item</div>
  <div>Normal</div>
  <div>Normal</div>
</div>
```

---

#### `.grid-stacked` / `.grid-stacked-3`

**Mobile-first stacked grid** that expands on larger screens.

- `.grid-stacked`: 1 column → 2 columns at 640px
- `.grid-stacked-3`: 1 column → 3 columns at 768px

```html
<div class="grid-stacked gap-md">
  <div>Stacks on mobile</div>
  <div>2 columns on tablet+</div>
</div>
```

---

### Fixed Grid Classes

#### `.grid-cols-*` (1-12)

Creates a grid with a **fixed number of columns**.

Available: `grid-cols-1`, `grid-cols-2`, `grid-cols-3`, `grid-cols-4`, `grid-cols-5`, `grid-cols-6`, `grid-cols-8`, `grid-cols-12`

```html
<div class="grid-cols-4 gap-md">
  <div>Column 1</div>
  <div>Column 2</div>
  <div>Column 3</div>
  <div>Column 4</div>
</div>
```

---

#### `.grid-rows-*` (2-5)

Creates a grid with a **fixed number of rows** with equal height.

Available: `grid-rows-2`, `grid-rows-3`, `grid-rows-4`, `grid-rows-5`

```html
<div class="grid-rows-3 gap-md" style="height: 400px;">
  <div>Row 1</div>
  <div>Row 2</div>
  <div>Row 3</div>
</div>
```

---

### Layout Pattern Classes

#### `.grid-sidebar` / `.grid-sidebar-sm` / `.grid-sidebar-lg`

Creates a **sidebar + main content** layout.

**Variants:**

- `.grid-sidebar-sm`: 200px sidebar
- `.grid-sidebar`: 300px sidebar (default)
- `.grid-sidebar-lg`: 400px sidebar

```html
<div class="grid-sidebar gap-lg">
  <aside>Sidebar</aside>
  <main>Main Content</main>
</div>
```

---

#### `.grid-sidebar-right`

Sidebar on the **right side** instead of left.

```html
<div class="grid-sidebar-right gap-lg">
  <main>Main Content</main>
  <aside>Sidebar</aside>
</div>
```

---

#### `.grid-sidebar-responsive`

Sidebar that **stacks on mobile** and appears side-by-side on larger screens (768px+).

```html
<div class="grid-sidebar-responsive gap-lg">
  <aside>Sidebar (stacks on mobile)</aside>
  <main>Main Content</main>
</div>
```

---

#### `.grid-holy-grail`

Classic **Holy Grail layout** (header, sidebars, content, footer).

**Required child classes:**

- `.grid-area-header`
- `.grid-area-sidebar-left`
- `.grid-area-content`
- `.grid-area-sidebar-right`
- `.grid-area-footer`

```html
<div class="grid-holy-grail">
  <header class="grid-area-header">Header</header>
  <aside class="grid-area-sidebar-left">Left Sidebar</aside>
  <main class="grid-area-content">Main Content</main>
  <aside class="grid-area-sidebar-right">Right Sidebar</aside>
  <footer class="grid-area-footer">Footer</footer>
</div>
```

---

#### `.grid-full-bleed`

Grid that allows items to **break out** to full width while keeping content centered.

Use `.full-width` class on items that should break out.

```html
<div class="grid-full-bleed">
  <h1>Normal Content (constrained)</h1>
  <p>Regular paragraph</p>
  <img class="full-width" src="hero.jpg" alt="Full width image" />
  <p>Back to constrained width</p>
</div>
```

---

#### `.grid-asymmetric` / `.grid-asymmetric-reverse`

Creates an **asymmetric 2-column layout** with custom ratio.

- `.grid-asymmetric`: 2:1 ratio (main content larger)
- `.grid-asymmetric-reverse`: 1:2 ratio (sidebar larger)

```html
<div class="grid-asymmetric gap-lg">
  <main>Main content (2/3 width)</main>
  <aside>Sidebar (1/3 width)</aside>
</div>
```

---

#### `.grid-masonry` / `.grid-masonry-4`

Creates a **masonry-style layout** effect.

- `.grid-masonry`: 3 columns
- `.grid-masonry-4`: 4 columns

**Note:** Items need inline `grid-row-end: span X` for varying heights.

```html
<div class="grid-masonry">
  <div style="grid-row-end: span 20;">Tall item</div>
  <div style="grid-row-end: span 10;">Short item</div>
  <div style="grid-row-end: span 15;">Medium item</div>
</div>
```

---

### Grid Item Classes

#### `.col-span-*` (1-6, full)

Makes a grid item **span across multiple columns**.

```html
<div class="grid-cols-4">
  <div class="col-span-2">Spans 2 columns</div>
  <div>Normal</div>
  <div>Normal</div>
</div>
```

---

#### `.row-span-*` (1-4, full)

Makes a grid item **span across multiple rows**.

```html
<div class="grid-cols-3">
  <div class="row-span-2">Tall item (2 rows)</div>
  <div>Normal</div>
  <div>Normal</div>
  <div>Normal</div>
  <div>Normal</div>
</div>
```

---

#### `.order-*`

Changes the **visual order** of grid items without changing HTML.

Available: `.order-first`, `.order-last`, `.order-1`, `.order-2`, `.order-3`

```html
<div class="grid-cols-3">
  <div class="order-last">Appears last</div>
  <div>Middle</div>
  <div class="order-first">Appears first</div>
</div>
```

---

### Alignment & Utility Classes

#### `.grid-center`

Centers content **both horizontally and vertically** within a grid cell.

```html
<div class="grid-center" style="min-height: 400px;">
  <h1>Perfectly Centered</h1>
</div>
```

---

#### Alignment Classes

Control **how items align** within their grid cells.

**Container alignment (affects all items):**

- `.items-start`, `.items-center`, `.items-end`, `.items-stretch`
- `.justify-items-start`, `.justify-items-center`, `.justify-items-end`, `.justify-items-stretch`

**Self alignment (affects single item):**

- `.self-start`, `.self-center`, `.self-end`, `.self-stretch`
- `.justify-self-start`, `.justify-self-center`, `.justify-self-end`

```html
<div class="grid-cols-3 items-center">
  <div>Centered vertically</div>
  <div class="self-start">Aligned to top</div>
  <div>Centered vertically</div>
</div>
```

---

#### Gap Classes

Control **spacing between grid items**.

**Uniform gaps:** `.gap-0`, `.gap-xs`, `.gap-sm`, `.gap-md`, `.gap-lg`, `.gap-xl`

**Directional gaps:** `.gap-x-*` (horizontal), `.gap-y-*` (vertical)

```html
<!-- Large uniform gap -->
<div class="grid-auto gap-lg">
  <div>Item 1</div>
  <div>Item 2</div>
</div>

<!-- Different horizontal and vertical gaps -->
<div class="grid-auto gap-x-lg gap-y-sm">
  <div>Wide horizontal space</div>
  <div>Narrow vertical space</div>
</div>
```

---

### Responsive Modifiers

Use **breakpoint prefixes** to apply classes at specific screen sizes.

**Breakpoints:**

- `sm:` - 640px and up
- `md:` - 768px and up
- `lg:` - 1024px and up

```html
<!-- 1 column mobile, 2 tablet, 4 desktop -->
<div class="grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-md">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
  <div>Item 4</div>
</div>

<!-- Responsive spanning -->
<div class="grid-cols-2 md:grid-cols-4">
  <div class="col-span-2 md:col-span-1">Full width mobile, 1/4 desktop</div>
  <div>Item 2</div>
  <div>Item 3</div>
  <div>Item 4</div>
</div>
```

---

## 💡 Usage Examples

### Responsive Image Gallery

```html
<div class="grid-auto-lg gap-lg">
  <img src="1.jpg" alt="Photo 1" />
  <img src="2.jpg" alt="Photo 2" />
  <img src="3.jpg" alt="Photo 3" />
  <img src="4.jpg" alt="Photo 4" class="col-span-2 row-span-2" />
  <img src="5.jpg" alt="Photo 5" />
  <img src="6.jpg" alt="Photo 6" />
</div>
```

---

### Dashboard Layout

```html
<div class="grid-sidebar gap-lg" style="min-height: 100vh;">
  <aside class="grid-rows-3 gap-md">
    <div>Navigation</div>
    <div>Menu</div>
    <div>Footer</div>
  </aside>

  <main class="grid-cols-3 gap-md">
    <div class="card">Widget 1</div>
    <div class="card">Widget 2</div>
    <div class="card">Widget 3</div>
    <div class="card col-span-2">Large Widget</div>
    <div class="card">Widget 5</div>
  </main>
</div>
```

---

### Blog Layout with Sidebar

```html
<div class="grid-sidebar-responsive gap-xl">
  <article class="grid-rows-3 gap-md">
    <header>Article Header</header>
    <div>Article Content</div>
    <footer>Article Footer</footer>
  </article>

  <aside>
    <div class="widget">Recent Posts</div>
    <div class="widget">Categories</div>
    <div class="widget">Newsletter</div>
  </aside>
</div>
```

---

### Product Grid with Featured Items

```html
<div class="grid-dense gap-md">
  <div class="product-card col-span-2 row-span-2">Featured Product</div>
  <div class="product-card">Product 2</div>
  <div class="product-card">Product 3</div>
  <div class="product-card">Product 4</div>
  <div class="product-card row-span-2">Tall Product</div>
  <div class="product-card">Product 6</div>
</div>
```

---

### Full-Width Hero Section

```html
<article class="grid-full-bleed gap-lg">
  <h1>Article Title</h1>
  <p>Introduction paragraph stays in content width</p>

  <img class="full-width" src="hero.jpg" alt="Full width hero" />

  <p>Back to regular content width</p>

  <div class="full-width highlight-section">
    <h2>Full width callout section</h2>
  </div>

  <p>More content...</p>
</article>
```

---
