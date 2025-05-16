# 🎯 Lightweight SCSS Utility Kit

A minimalist alternative to heavy CSS frameworks, providing only the most useful utility classes from Bootstrap without the bloat.

## Overview

This lightweight SCSS toolkit gives you the most commonly used utility classes for spacing, grid layout, typography, layout positioning, flex utilities, and basic components without forcing you to include an entire CSS framework. Perfect for projects where you need flexibility with minimal overhead.

## Installation

### 🔧 Prerequisites

To use this kit, ensure your project has the following:

- A working [Next.js 13+](https://nextjs.org/docs/app/building-your-application/routing/pages-and-layouts) or modern frontend setup
- `sass` installed as a dependency

```bash
npm install sass
```

### 📁 Folder Structure

This SCSS utility kit is structured around the following directory:

```
/styles
│
├── abstracts
│   ├── _breakpoints.scss
│   └── _spacing.scss
│
├── components
│   └── _button.scss
│
├── layout
│   ├── _columns.scss
│   ├── _container.scss
│   └── _grid.scss
│
├── utilities
│   ├── _display.scss
│   ├── _flex.scss
│   ├── _gap.scss
│   ├── _inset_.scss
│   ├── _list_.scss
│   ├── _position_.scss
│   ├── _sizing.scss
│   ├── _text.scss
│
└── main.scss
```

### 🔌 Usage

Import `main.scss` into your project’s root layout file (`layout.tsx`) or a global entry point such as `globals.scss`:

```ts
import '@/styles/main.scss';
```

## Features

### 🛆 Flex Utilities

Build flexible and responsive layouts using utility classes for flexbox:

- Display: `.d-flex`, `.d-inline-flex`
- Direction: `.flex-row`, `.flex-column`, `.flex-row-reverse`, `.flex-column-reverse`
- Wrap: `.flex-wrap`, `.flex-nowrap`, `.flex-wrap-reverse`
- Justify Content: `.justify-content-start`, `.justify-content-center`, `.justify-content-end`, `.justify-content-between`, `.justify-content-around`, `.justify-content-evenly`
- Align Items: `.align-items-start`, `.align-items-center`, `.align-items-end`, `.align-items-baseline`, `.align-items-stretch`
- Align Self: `.align-self-start`, `.align-self-center`, `.align-self-end`, `.align-self-stretch`

### 🛆 Grid System

A responsive, mobile-first flexbox grid system to build layouts of all shapes and sizes:

- `.container` - A centered, width-restricted wrapper
- `.row` - Flexbox container for columns
- `.col-1` through `.col-12` - Column widths on a 12-column grid
- Responsive variants: `.col-sm-*`, `.col-md-*`, `.col-lg-*`, `.col-xl-*`, `.col-xxl-*`

### 🖐️ Spacing Utilities

Comprehensive margin and padding utilities for consistent spacing:

- Margin: `.m-*`, `.mt-*`, `.mb-*`, `.ms-*`, `.me-*`, `.mx-*`, `.my-*`
- Padding: `.p-*`, `.pt-*`, `.pb-*`, `.ps-*`, `.pe-*`, `.px-*`, `.py-*`

Where `*` represents size values from 0 to 5, using a consistent spacing scale.

### 🅰️ Text Utilities

Utilities for text alignment, transformation, weight, and color:

- Alignment: `.text-left`, `.text-center`, `.text-right`
- Transformation: `.text-uppercase`, `.text-lowercase`, `.text-capitalize`
- Weight: `.fw-light`, `.fw-normal`, `.fw-medium`, `.fw-bold`
- Size: `.fs-1` through `.fs-8` (smallest to largest)
- Color: `.text-primary`, `.text-secondary`, `.text-success`, `.text-danger`, `.text-muted`

### 🔘 Button Styles

Simple button styles for common actions:

- `.btn` - Base button style
- `.btn-primary` - Emphasized primary action
- `.btn-outline` - Secondary outline style
- `.btn-disabled` - Disabled state

```html
<button class="btn btn-primary">Save</button>
<button class="btn btn-outline">Cancel</button>
```

### 📍 Position Utilities

Helpers for absolute/relative positioning and directional placement:

- Position: `.position-static`, `.position-relative`, `.position-absolute`, `.position-fixed`, `.position-sticky`
- Offsets: `.top-0`, `.bottom-0`, `.start-0`, `.end-0`

### 📏 Sizing Utilities

Quick width and height control:

- Width: `.w-100`, `.w-75`, `.w-50`, `.w-25`
- Height: `.h-100`, `.h-75`, `.h-50`, `.h-25`

### 📝 List Utilities

Remove default list styles:

- `.list-unstyled` - Removes bullets and default padding

### 🪩 Breakpoints

Standard responsive breakpoints for consistent behavior:

- `xs`: 0px
- `sm`: 576px
- `md`: 768px
- `lg`: 992px
- `xl`: 1200px
- `xxl`: 1400px

## Why Use This Instead of a Full Framework?

- **Performance**: Significantly smaller file size compared to full frameworks
- **Simplicity**: Only the most commonly used utilities, no complex components
- **Flexibility**: Easier to customize without fighting against existing styles
- **Learning Curve**: Familiar naming conventions if you know Bootstrap
- **Minimal Dependencies**: No JavaScript dependencies required

## Browser Support

Compatible with all modern browsers (Chrome, Firefox, Safari, Edge).

## Contributing

Contributions are welcome to help and improve the Lightweight SCSS Utility Kit!

If you find a bug, want to suggest an enhancement, or add new utility classes, feel free to open an issue or submit a pull request.

### 🛠 How to Contribute

1. **Fork the repository**
2. **Create a new branch** for your feature or fix:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**, and make sure your code follows existing formatting and naming conventions
4. **Test your changes** by running your local dev environment
5. **Commit** and push your changes:

   ```bash
   git commit -m "Add: description of your change"
   git push origin feature/your-feature-name
   ```

6. **Create a pull request** from your forked repository

### ✍️ Contribution Guidelines

- Keep utility naming consistent with Bootstrap-style conventions (`.fs-1`, `.btn-primary`, etc.)
- Do not include JavaScript-based components — this kit is purely SCSS-focused
- Avoid adding unnecessary styles or classes that duplicate existing utilities
- Group similar utilities together for better maintainability
- Make sure your code is clean and documented when necessary

---

**Lightweight SCSS Utility Kit**
All the utilities you need, none of the bloat you don't.
