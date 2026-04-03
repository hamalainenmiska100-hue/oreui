# Ore UI Core

This repository contains the core Ore UI web assets.

## Structure

/dist/
/assets/

Do not rename or modify these folders.

---

## How to use

This repository is designed to be used via jsDelivr CDN, not locally.

### Base CDN URL

https://cdn.jsdelivr.net/gh/hamalainenmiska100-hue/oreui@main/

---

## Required HTML setup

Use these exact CDN links in your <head>:

<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/hamalainenmiska100-hue/oreui@main/dist/preload.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/hamalainenmiska100-hue/oreui@main/dist/libs/main.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/hamalainenmiska100-hue/oreui@main/dist/libs/buttons.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/hamalainenmiska100-hue/oreui@main/dist/libs/input.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/hamalainenmiska100-hue/oreui@main/dist/libs/icons.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/hamalainenmiska100-hue/oreui@main/dist/libs/fonts.css">

<script type="module" src="https://cdn.jsdelivr.net/gh/hamalainenmiska100-hue/oreui@main/dist/lite.init.js"></script>

---

## Critical rules

1. Always use CDN paths

Do NOT use:
./dist/...
./assets/...

Always use:
https://cdn.jsdelivr.net/gh/hamalainenmiska100-hue/oreui@main/...

---

2. Use lite.init.js

Do NOT use all.init.js

---

3. Always remove the loader

<script>
window.addEventListener("load", () => {
  const loader = document.querySelector("loader")
  if (loader) loader.style.display = "none"
})
</script>

---

## What Ore UI is

Ore UI is primarily:
- a CSS design system
- UI components and styles

It is NOT a reliable JavaScript framework.

---

## Recommended usage

- Use Ore UI for styling only
- Write your own JavaScript logic
- Avoid relying on built-in JS behavior

---

## Known issues

- all.init.js can freeze the page
- fonts may fail if incorrectly loaded
- some components depend on unstable JS

---

## Production tip

Use versioned CDN links when possible.

---

## Summary

- Use jsDelivr CDN
- Do not use local paths
- Use lite.init.js
- Hide loader manually

This repository is intended as a reusable UI base (e.g. for DeepSeed).
