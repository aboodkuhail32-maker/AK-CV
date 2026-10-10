# 01 — Overview

## What you made

A **one-page portfolio / CV website** that advertises you as a
**Roblox developer for hire**, under the name **-AK-** (Discord: `its_47_`).

The page tells visitors:

- Who you are: a multi-skilled Roblox developer with **3+ years of experience**
- What you do: **Scripting (Lua/Luau), Building & Mapping, GUI Design, Clothing Design**
- What kind of games you're best for: RP, open world, military, survival, simulators, custom projects
- Your time zone: **Saudi Arabia, AST (UTC+3)**
- How you get paid: **Robux only, minimum 70 Robux**, price based on the work
- How to hire you: **DM on Discord**

## Timeline (from git history)

| Date | What happened |
|------|---------------|
| 9 May 2026 | Uploaded `ak-roblox-cv_1.html` (the website) |
| 9 May 2026 | Uploaded the same page again as `index.html.html` |
| 26 Sep 2026 | Deleted `ak-roblox-cv_1.html` |
| 26 Sep 2026 | Deleted `index.html.html` |

Both files were **identical** (493 lines each). Right now the repository has no
website files in it, only this guide.

## Getting the website back

The deleted file is still saved in git history. To restore it:

```bash
git checkout 652d192 -- index.html.html
git mv index.html.html index.html   # optional: fix the double ".html" name
```

> Tip: if you want to host it for free with **GitHub Pages**, the file should be
> called `index.html` (not `index.html.html`). Then turn on Pages in the repo
> settings → Pages → deploy from branch `main`.

## How it is built

The whole website is **one single HTML file**. It has:

1. **HTML** for the content (text, sections, buttons)
2. **CSS** inside a `<style>` tag for the look and animations
3. **JavaScript** inside a `<script>` tag for the moving background and effects

No frameworks, no build step, no images. Everything (even the avatar "AK"
logo) is drawn with code, so it loads fast and works by just opening the file.
