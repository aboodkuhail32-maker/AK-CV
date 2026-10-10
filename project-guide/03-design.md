# 03 — Design

## Color palette

All colors are defined once at the top of the CSS (`:root`) so they are easy to change.

| Name | Hex | Used for |
|------|-----|----------|
| `--bg` | `#06080e` | Main page background (almost black) |
| `--bg2` / `--bg3` / `--bg4` | `#0b0e18` / `#10141f` / `#151a28` | Cards and panels, slightly lighter |
| `--text` | `#eef0f8` | Main text |
| `--muted` / `--muted2` | `#6b7399` / `#8b90b3` | Secondary text |
| `--cyan` | `#00e5ff` | Main brand color: buttons, highlights, particles |
| `--purple` | `#a855f7` | Gradients, GUI Design card |
| `--orange` | `#f97316` | Gradients, Scripting card |
| `--green` | `#22d3a0` | "Available" dot, "Open to hire" badge, Building card |
| `--amber` | `#fbbf24` | Payment highlights |
| Discord blue | `#5865F2` | The Discord button |

The style is a **dark "gamer / tech" theme** with neon glows.

## Fonts

- **Syne** (weights 400–800): big bold headings, logo, buttons, numbers
- **Outfit** (weights 300–600): normal paragraph text

## Page sections (top to bottom)

1. **Navigation bar**: the `-AK-` logo, links (Services, Why Me, Payment, Contact),
   a blinking green "Available for hire" dot and a cyan **Hire Me →** button.
   It slides down when the page loads and has a blurred glass background.
2. **Hero**: the big headline *"Building worlds. One script at a time."*, a short
   intro, skill tags, and two buttons. On the right is the **AK avatar** with a
   spinning rainbow border, a scanning light line, three floating emojis
   (⚡ 🎮 🛠️) and an "✦ Open to hire" badge.
3. **Stats**: three numbers that count up: **3+** years, **4** disciplines, **70+** starting Robux.
4. **Time zone card**: "Working on Saudi Arabia Time · UTC+3 · AST".
5. **Services**: four cards, each with its own color:
   - 🎨 Clothing Design (cyan)
   - 🏗️ Building & Mapping (green)
   - 🖥️ GUI Design (purple)
   - ⚡ Scripting Lua/Luau (orange)
6. **Why work with me?**: five ✓ points (detail, quality and performance, solo or team, creative ideas, polished work).
7. **Best for**: chips for RP, Open World, Military, Survival, Simulator, Custom projects.
8. **Payment**: Robux only · minimum 70 Robux · based on work.
9. **Contact (CTA)**: "Ready to build something great?" with the Discord buttons.
10. **Footer**: name, Discord username `its_47_`, user ID and time zone.

## Hover effects

Almost every card reacts when you hover: it lifts up (`translateY`), slides
right (`translateX`) or grows (`scale`), and its border or glow lights up.

## Mobile layout

Below 960px wide: nav links hide, the hero stacks vertically and centers,
and all grids become a single column.
