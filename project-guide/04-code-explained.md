# 04 — Code Explained

The JavaScript at the bottom of the page has **4 small parts**. Each one is
wrapped in `(function(){ ... })();` so its variables don't clash with the others.

---

## 1. Particle background

Draws the moving dots and lines behind everything on a full-screen `<canvas>`.

**How it works:**

1. **Size**: the canvas is made the size of the window, and resizes with it.
2. **Create particles**: the number of dots depends on screen size
   (`width × height / 14000`). Each dot gets a random:
   - position (`x`, `y`)
   - slow speed (`vx`, `vy` between -0.18 and 0.18)
   - size (0.5 to 2 px)
   - opacity (0.08 to 0.45)
   - color: cyan, purple or white
3. **Every frame** (`requestAnimationFrame`):
   - Clear the canvas
   - Draw a faint **grid** of lines every 70 px
   - Move each dot. If it leaves the screen it wraps around to the other side
   - **Mouse attraction**: if the mouse is closer than 200 px, the dot is pulled slightly toward it
   - Draw each dot as a small circle
   - **Connections**: for every pair of dots closer than 110 px, draw a thin cyan line.
     The closer they are, the brighter the line.

---

## 2. Scroll reveal

Elements with the class `reveal` start invisible and 44 px lower.
An `IntersectionObserver` watches them. When 10% of one is on screen, it adds
the class `vis`, and CSS animates it to full opacity at its normal position.

Classes `d1`…`d5` add small delays (0.08s → 0.48s) so cards in a row appear
one after another instead of all at once.

---

## 3. Count-up numbers

The stat numbers have attributes like `data-target="70" data-suffix="+"`.
When a number scrolls into view:

- It animates from 0 to the target over **1.6 seconds**
- It uses an **ease-out curve** (`1 - (1-p)³`), so it starts fast and slows down at the end
- Then it adds the suffix, like `+`

---

## 4. Cursor glow

Creates an invisible 320 px circle with a soft cyan radial gradient that
follows the mouse, giving a subtle "flashlight" glow wherever you point.

---

## CSS animations

| Name | What it does |
|------|--------------|
| `slideDown` | Nav bar slides in from the top on load |
| `fadeUp` | Hero text, tags and buttons fade up one by one (staggered delays) |
| `blink` | The green "available" dot pulses |
| `spin` | Rotates the rainbow border around the avatar (7s per turn) |
| `scan` | A thin cyan line moves down over the avatar like a scanner |
| `float` | The ⚡ 🎮 🛠️ emojis bob up and down |

---

## Small things worth fixing if you bring the site back

- Rename `index.html.html` to `index.html` so GitHub Pages and browsers treat it normally.
- The "Hire Me" links go to `discord.com/channels/@me/<id>`, which only works if
  the visitor already has a DM open with you. The "View Discord Profile" link
  (`discord.com/users/<id>`) works for everyone, so it's the safer link for all buttons.
