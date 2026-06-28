# CLT (CSS Library Tools)

A lightweight CSS and JavaScript library focused on productivity, simplicity, and customization.

---

# About

CLT (CSS Library Tools) was created to speed up front-end development using native HTML, CSS, and JavaScript.

Instead of replacing the way you build websites, CLT automates repetitive tasks while keeping your code clean, readable, and easy to customize.

The library combines modern CSS, lightweight JavaScript, and native browser features to create responsive interfaces with minimal code.

---

# Features

* **Theme System:** Fully powered by CSS Variables.
* **Component-Driven:** Ready-to-use structural and UI elements.
* **Smart JS Helpers:** Native script automation without boilerplate.
* **Automatic Floating Labels:** Generated automatically using the `clt` attribute.
* **Password Reveal:** Built-in toggle functionality for password inputs.
* **Button States:** Supports active, disabled, and loading states.
* **Automatic Alerts:** Custom `<clt-alert>` elements ready to use.
* **Utility Helpers:** Built-in Copy to Clipboard and File Download helpers.
* **Responsive Layouts:** Flexible containers and structural components.
* **Custom Scrollbar:** Styled scrollbars with a minimalist design.
* **Scroll Reveal Animation:** Animate elements as they enter the viewport.
* **Zero Dependencies:** Built entirely with native HTML, CSS and JavaScript.

---

# Installation

## Local Installation

Include the required files inside your project.

```html
<link rel="stylesheet" href="clt-dark-minimalist.css">
<link rel="stylesheet" href="clt.min.css">

<script src="clt-functions.js"></script>
```

---

## Public Usage (CDN)

You can also use CLT directly from the hosted version without downloading any files.

```html
<link rel="stylesheet" href="https://clt-iota.vercel.app/clt-dark-minimalist.css">
<link rel="stylesheet" href="https://clt-iota.vercel.app/clt.min.css">

<script src="https://clt-iota.vercel.app/clt-functions.js"></script>
```

This is the recommended option for quick prototypes and small projects.

---

# Components

## Card

```html
<div class="clt-card">
    <h2 class="clt-card-title">
        Card Title
    </h2>

    <p class="clt-card-text">
        Card text.
    </p>

    <button class="clt-card-button">
        Button
    </button>
</div>
```

---

## Typography & Links

### Title

```html
<h1 class="clt-title">
    Hello World
</h1>
```

### Paragraph

```html
<p class="clt-p">
    Paragraph.
</p>
```

### Link

```html
<a href="#" class="clt-link">
    Link
</a>
```

---

## Inputs & Forms

### Smart Input

Simply use the `clt` attribute.

```html
<input clt="Name">
```

CLT automatically generates:

* Floating Label
* Input Group
* Placeholder
* Responsive layout

### Password Reveal

```html
<input
type="password"
clt="Password"
reveal>
```

Adding the `reveal` attribute automatically creates a show/hide password control.

---

## Buttons & States

### Default

```html
<button class="clt-card-button">
    Button
</button>
```

### Active

```html
<button class="clt-card-button" clt="on">
    Button
</button>
```

### Disabled

```html
<button class="clt-card-button" clt="off">
    Button
</button>
```

### Loading

```html
<button class="clt-card-button" clt="loading">
    Loading...
</button>
```
---

## Alerts

### Default

```html
<clt-alert>
    Message
</clt-alert>
```

### Warning

```html
<clt-alert type="warn">
    Message
</clt-alert>
```

### Danger

```html
<clt-alert type="alert">
    Message
</clt-alert>
```

---

## Loader

```html
<div class="clt-loader"></div>
```

---

# JavaScript Helpers

CLT provides built-in JavaScript helpers to reduce repetitive code while keeping your HTML clean.

---

## Copy to Clipboard

Copy the text content of any element using its ID.

```html
<pre id="example-code">
Hello World
</pre>

<button
class="clt-card-button"
clt-copy="example-code">
    Copy
</button>
```

When clicked, CLT automatically copies the element content to the user's clipboard.

---

## File Download

Trigger downloads without writing JavaScript.

```html
<button
class="clt-card-button"
clt-download="clt-v1.0.zip">
    Download
</button>
```

Custom filename:

```html
<button
class="clt-card-button"
clt-download="downloads/library.zip"
download-name="CLT.zip">
    Download
</button>
```

---

# Layout Components

## Header

```html
<header class="clt-header"></header>
```

---

## Navbar

```html
<nav class="clt-navbar"></nav>
```

---

## Main

```html
<main class="clt-main"></main>
```

---

## Section

```html
<section class="clt-section"></section>
```

---

## Container

```html
<div class="clt-container"></div>
```

---

## Center

```html
<div class="clt-center"></div>
```

or

```html
<div class="clt-flex-center"></div>
```

---

## Footer

```html
<footer class="clt-footer">
    <p class="clt-footer-text">
        Footer
    </p>

    <p class="clt-footer-right">
        Loaden TI
    </p>
</footer>
```

---

# Scroll Animation

Apply the class to the `<body>` element.

```html
<body class="clt-animation-scroll">
```

Every direct child element will smoothly animate when entering the viewport.

---

# Customization

CLT is entirely powered by CSS Variables.

You can override any variable inside your own `:root` without modifying the library source files.

Example:

```css
:root{
    --clt-surface:#202020;
    --clt-text:#ffffff;
    --clt-border-color:#00aaff;
}
```

This allows complete theme customization while keeping future updates simple.

---

# Boilerplate

A ready-to-use HTML template for starting new projects with CLT.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CLT Project</title>

    <link rel="stylesheet" href="clt-dark-minimalist.css">
    <link rel="stylesheet" href="clt.min.css">
</head>

<body class="clt-animation-scroll">

    <nav class="clt-navbar">
        <h1 class="clt-title">My App</h1>
    </nav>

    <main class="clt-main">

        <div class="clt-container clt-flex-center">

            <div class="clt-card">

                <h2 class="clt-card-title">
                    Welcome
                </h2>

                <p class="clt-card-text">
                    Start building your interface.
                </p>

                <input clt="Email">

                <input
                type="password"
                clt="Password"
                reveal>

                <button class="clt-card-button">
                    Get Started
                </button>

            </div>

        </div>

    </main>

    <footer class="clt-footer">
        <p class="clt-footer-text">
            © 2026 My Project
        </p>

        <p class="clt-footer-right">
            Powered by CLT
        </p>
    </footer>

    <script src="clt-functions.js"></script>

</body>
</html>
```

---

# Download

## Website

```
https://clt-iota.vercel.app
```

---

## GitHub Repository

```
https://github.com/Bugzin-xD/CLT-CSS-Library-Tools-
```

---

# Philosophy

CLT follows four core principles.

* **Simplicity** — Clean, lightweight and easy to understand.
* **Performance** — Native rendering with zero dependencies.
* **Native Integration** — Works with HTML instead of replacing it.
* **Customization** — Everything is customizable through CSS Variables.

CLT was designed to help developers build interfaces faster without hiding how HTML, CSS and JavaScript work.

---

# Browser Support

Recommended browsers:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox
* Opera
* Brave

---

# License

Copyright © Loaden TI.

All rights reserved.
