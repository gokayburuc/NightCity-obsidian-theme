# Night City — Obsidian Cyberpunk Theme

**Night City** is a cyberpunk-inspired theme for [Obsidian](https://obsidian.md), drawing visual language from *Cyberpunk 2077* and *Cyberpunk: Edgerunners*: neon glow, glitch accents, scanlines, and cut-corner HUD frames.

![Palette](https://img.shields.io/badge/palette-071a23%20%200a2431%20%2019465a%20%203f8493-071a23)

## ✨ Features

- **Michroma** typeface (Google Fonts) across the entire UI — headings, body text, and interface
- **Neon-yellow headings** (H1–H6) with layered glow and a red glitch pulse on hover
- **Futuristic callouts** with scanline strips and cut-corner (clip-path) frames:
  - `info` / `note` — **NETRUNNER** (teal terminal)
  - `tip` — **BRIGHT IDEA** (yellow glitch)
  - `success` — **JACKED IN** (green uplink)
  - `warning` — **CYBERPSYCHO** (gold, animated flicker)
  - `danger` / `error` / `bug` — **FLATLINE** (red emergency)
  - `quote` / `abstract` — chrome dossier
- **Styled emphasis**: bold = neon yellow, italic = red, underline = green, strikethrough = gold
- **Neon tables** with yellow uppercase headers, teal borders, and gold hover edges
- **Bright tags** — yellow neon pills that flash red on hover
- **Glowing properties/frontmatter panel** — gold keys, green values
- Neon inline note title, scanline horizontal rules, teal-dashed internal links, and an active-line rail in the editor

## 🎨 Color Palette

| Role | Hex |
| --- | --- |
| Deep background | `#071a23` |
| Panel background | `#0a2431` |
| Raised surface | `#19465a` |
| Accent teal | `#3f8493` |
| Neon yellow | `#e8df06` |
| Alert red | `#be021b` |
| Uplink green | `#94d788` |
| Signal gold | `#e5b12d` |
| Body text (pastel yellow) | `#746f02` |

## 📦 Installation

### From vault (manual)

1. In your vault, create the folder `.obsidian/themes/Night City/`
2. Copy `theme.css` into that folder
3. Add a `manifest.json` next to it:

```json
{
  "name": "Night City",
  "version": "1.0.0",
  "minAppVersion": "1.0.0",
  "author": "Gokay BURUC"
}
```

4. Restart Obsidian
5. Go to **Settings → Appearance → Themes** and select **Night City**

### From Community Themes (optional)

If you want to publish the theme, submit a PR to the [obsidianmd/obsidian-releases](https://github.com/obsidianmd/obsidian-releases) repository following the [official theme guide](https://docs.obsidian.md/Themes/App+themes/Build+a+theme).

## 🔤 Fonts

Michroma is loaded from Google Fonts via `@import`:

```css
@import url('https://fonts.googleapis.com/css2?family=Michroma&display=swap');
```

> **Note:** This requires an internet connection. For fully offline use, download Michroma into your vault and register it with `@font-face`, then replace the `@import` line.

## 🧩 Customization

All colors are defined once as CSS variables at the top of `theme.css`:

```css
:root {
  --nc-bg-deep:   #071a23;
  --nc-bg-panel:  #0a2431;
  --nc-bg-raised:#19465a;
  --nc-teal:      #3f8493;
  --nc-yellow:    #e8df06;
  --nc-red:       #be021b;
  --nc-green:     #94d788;
  --nc-gold:      #e5b12d;
  --nc-text:      #746f02;
}
```

Tweak these to re-skin the entire theme without touching component styles.

## ⚠️ Known Quirks

- Michroma is wide and geometric — very long words in headings may wrap more often than with standard fonts
- The `CYBERPSYCHO` (warning) callout title has a subtle flicker animation; remove the `nc-flicker` animation if you prefer a static title
- Light mode is intentionally minimal; the theme is designed for dark mode

## 📄 License

MIT — do whatever you want, credit appreciated.
