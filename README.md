# Shop Cart — Knockout.js

A small, single-page shopping cart app built with **Knockout.js** to demonstrate core MVVM concepts: observables, computed properties, and declarative data-binding.

## Live Demo

Open `shop-cart-knockout.html` directly in any browser — no build step, no server, no dependencies to install.

## Features

- Browse a small product catalog and add items to a cart
- Adjust quantity with `+` / `−` controls, or remove an item entirely
- Live-updating item count, subtotal, tax, and total
- Checkout button that clears the cart and shows a confirmation message
- Fully responsive layout (mobile and desktop)

## Tech Stack

- [Knockout.js](https://knockoutjs.com/) 3.5.1 (via CDN)
- Vanilla HTML/CSS/JS — no build tools, no frameworks beyond Knockout

## Concepts Demonstrated

| Concept | Where it's used |
|---|---|
| `ko.observable()` | Cart state, order confirmation, item quantities |
| `ko.observableArray()` | The cart list itself |
| `ko.computed()` | Cart count, subtotal, tax, and total — all derived automatically |
| `foreach` binding | Rendering the product grid and cart items |
| `click` binding | Add to cart, quantity controls, remove, checkout |
| `text` / `visible` / `enable` bindings | Displaying values, toggling UI states, disabling checkout when empty |
| `$parent` context | Calling parent view-model methods from inside a `foreach` loop |
| Composed view models | Each cart item wraps a product object with its own observable quantity |

## Project Structure

```
shop-cart-knockout.html   # entire app: HTML, CSS, and JS in one file
README.md                 # this file
```

## Why a Single File?

This project is intentionally scoped small — a focused demo of Knockout.js fundamentals rather than a full production build. Keeping everything in one file makes it easy to open, read top to bottom, and review in a few minutes.

## Author

Built as a hands-on exercise to learn and demonstrate Knockout.js's MVVM pattern and data-binding system.
