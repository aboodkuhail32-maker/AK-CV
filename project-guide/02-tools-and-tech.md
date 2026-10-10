# 02 — Tools & Tech Used

## Languages

| Language | Used for |
|----------|----------|
| **HTML5** | The structure of the page: nav bar, hero, stats, services, payment, contact, footer |
| **CSS3** | Colors, layout (Flexbox + Grid), gradients, glass blur, animations, mobile layout |
| **JavaScript (vanilla)** | Particle background, scroll animations, number count-up, cursor glow |
| **SVG** | The Discord logo inside the "Message on Discord" button |

## External services

| Service | Why |
|---------|-----|
| **Google Fonts** | Loads the two fonts: **Syne** (headings) and **Outfit** (body text) |
| **Discord** | All "Hire Me" / "DM" buttons link to your Discord DM and profile |
| **GitHub** | Stores the project (this repository) |

## Browser features used

| Feature | Where |
|---------|-------|
| `<canvas>` + 2D context | Drawing the animated particle network in the background |
| `requestAnimationFrame` | Smooth 60fps animation loop for particles and counters |
| `IntersectionObserver` | Detects when a section scrolls into view, to fade it in and start the counters |
| CSS custom properties (`--cyan`, etc.) | One place to change every color on the site |
| `backdrop-filter: blur()` | The frosted-glass look of the top navigation bar |
| `background-clip: text` | The gradient-colored headline text and stat numbers |
| `conic-gradient` | The spinning rainbow border around the "AK" avatar |
| `@media (max-width:960px)` | Makes the page work on phones and tablets |
| `scroll-behavior: smooth` | Smooth scrolling when clicking nav links |

## Emojis used as icons

Instead of image files, the page uses emojis as icons:
⚡ 🏗️ 🎨 🖥️ 🕐 💬 🎮 🛠️ 🕌 💰 📊 📋 ✓ ✦
