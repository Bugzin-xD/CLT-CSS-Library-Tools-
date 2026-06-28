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
* **Automatic Floating Labels:** Handled automatically via attributes.
* **Password Reveal:** Built-in toggle functionality for password inputs.
* **Button States:** Dedicated attributes for active, disabled, and loading states.
* **Automatic Alerts:** Custom alert elements ready out of the box.
* **Utility Helpers:** Fast setup for Copy to Clipboard and File Downloads.
* **Responsive Layouts:** Flexible grid and container systems.
* **Aesthetics:** Custom scrollbars and scroll-reveal animations.
* **Performance:** Zero external dependencies.

---

# Installation

Include the required files in the `<head>` and at the end of the `<body>` of your project:

```html
<!-- Inside <head> -->
<link rel="stylesheet" href="clt-dark-minimalist.css">
<link rel="stylesheet" href="clt.min.css">

<!-- Before </body> closes -->
<script src="clt-functions.js"></script>
```

---

# Components

## Card

```html
<div class="clt-card">
    <h2 class="clt-card-title">Card Title</h2>
    <p class="clt-card-text">Card text.</p>
    <button class="clt-card-button">Button</button>
</div>
```

---

## Typography & Links

### Title
```html
<h1 class="clt-title">Hello World</h1>
```

### Paragraph
```html
<p class="clt-p">Paragraph.</p>
```

### Link
```html
<a class="clt-link">Link</a>
```

---

## Inputs & Forms

### Smart Input
Simply use the `clt` attribute to automatically generate a Floating Label, Input Group, Responsive layout, and Placeholder:

```html
<input clt="Name">
```

### Password Reveal
Automatically creates a show/hide password control by adding the `reveal` attribute:

```html
<input type="password" clt="Password" reveal>
```

---

## Buttons & States

### Default
```html
<button class="clt-card-button">Button</button>
```

### Active
```html
<button class="clt-card-button" clt="on">Button</button>
```

### Disabled
```html
<button class="clt-card-button" clt="off">Button</button>
```

### Loading
```html
<button class="clt-card-button" clt="loading">Loading...</button>
```

---

## Alerts

### Default
```html
<clt-alert>Message</clt-alert>
```

### Warning
```html
<clt-alert type="warn">Message</clt-alert>
```

### Danger
```html
<clt-alert type="alert">Message</clt-alert>
```

---

## Loader

```html
<div class="clt-loader"></div>
```

---

## JavaScript Helpers

### Copy to Clipboard
Easily copy the text contents of any element by referencing its ID:

```html
<pre id="example-code">Hello World</pre>

<button class="clt-card-button" clt-copy="example-code">Copy</button>
```

### Download Helper
Trigger local file downloads instantly:

```html
<button class="clt-card-button" clt-download="clt-v1.0.zip">Download</button>
```

You can also specify a custom download name:

```html
<button class="clt-card-button" clt-download="downloads/library.zip" download-name="CLT.zip">Download</button>
```

---

## Layout & Structure

### Navigation & Headers
```html
<header class="clt-header"></header>
<nav class="clt-navbar"></nav>
```

### Main Structure
```html
<main class="clt-main"></main>
<section class="clt-section"></section>
<div class="clt-container"></div>
```

### Centering Elements
```html
<div class="clt-center"></div>
<!-- or -->
<div class="clt-flex-center"></div>
```

### Footer
```html
<footer class="clt-footer">
    <p class="clt-footer-text">Footer</p>
    <p class="clt-footer-right">Loaden TI</p>
</footer>
```

---

## Scroll Animation

Apply the class to the `<body>` tag, and every direct child element will smoothly animate when entering the viewport:

```html
<body class="clt-animation-scroll">
```

---

# Customization

CLT is entirely powered by CSS Variables. You can override any variable inside your own `:root` file without touching the core library files.

Example:

```css
:root {
    --clt-surface: #202020;
    --clt-text: #ffffff;
    --clt-border-color: #00aaff;
}
```


---

# Boilerplate

Here is a ready-to-use HTML template containing the basic structure to start developing with CLT instantly:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CLT Project Template</title>
    
    <!-- CLT CSS Stylesheets -->
    <link rel="stylesheet" href="clt-dark-minimalist.css">
    <link rel="stylesheet" href="clt.min.css">
</head>
<body class="clt-animation-scroll">

    <!-- Navbar -->
    <nav class="clt-navbar">
        <h1 class="clt-title">My App</h1>
    </nav>

    <!-- Main Container -->
    <div class="clt-container clt-flex-center">
        <main class="clt-main">
            <div class="clt-card">
                <h2 class="clt-card-title">Welcome to CLT</h2>
                <p class="clt-card-text">Start building your clean interface here.</p>
                
                <!-- Smart Form Example -->
                <input clt="Email Address">
                <input type="password" clt="Password" reveal>
                
                <button class="clt-card-button">Get Started</button>
            </div>
        </main>
    </div>

    <!-- Footer -->
    <footer class="clt-footer">
        <p class="clt-footer-text">© 2026 My Project</p>
        <p class="clt-footer-right">Powered by CLT</p>
    </footer>

    <!-- CLT JavaScript Functions -->
    <script src="clt-functions.js"></script>
</body>
</html>
```

---

# To use

* **Install in the website/Github**
* **Use with link**
  
# Links
* **clt.min.css**: *clt-iota.vercel.app/clt.min.css*
* **clt-dark-minimalist.css**: *clt-iota.vercel.app/clt-dark-minimalit.css*

---

# Download
* **Website**: *clt-iota.vercel.app*
* **Github**: The zip archive

---

# Philosophy

CLT follows four core principles:
* **Simplicity:** Keep it clean, lightweight, and easy to understand.
* **Performance:** High-speed rendering with native tech and zero dependencies.
* **Native Integration:** Works with your workflow, not against it.
* **Customization:** Full control over themes via CSS Variables.

---

# Browser Support

Recommended and tested modern browsers:
* Google Chrome
* Microsoft Edge
* Mozilla Firefox
* Opera
* Brave

---

# License

Copyright © Loaden TI. All rights reserved.
