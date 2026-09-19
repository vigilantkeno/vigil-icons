# Vigil Icons

<p>
  <img src="https://www.vigilicons.com/icons/ghosting.png" width="56" alt="Ghosting">
  <img src="https://www.vigilicons.com/icons/red-flag.png" width="56" alt="Red flag">
  <img src="https://www.vigilicons.com/icons/situationship.png" width="56" alt="Situationship">
  <img src="https://www.vigilicons.com/icons/gaslighting.png" width="56" alt="Gaslighting">
  <img src="https://www.vigilicons.com/icons/cooked.png" width="56" alt="Cooked">
  <img src="https://www.vigilicons.com/icons/the-ick.png" width="56" alt="The ick">
  <img src="https://www.vigilicons.com/icons/mid.png" width="56" alt="Mid">
  <img src="https://www.vigilicons.com/icons/couldve-been-an-email.png" width="56" alt="Could've been an email">
</p>

**111 icons for the vocabulary people actually use about each other.** Gaslighting, ghosting, red
flag, situationship, main character syndrome, could've been an email. General-purpose icon sets have
folders and arrows; nobody had drawn these, and the emoji keyboard does not cover them either.

All 111 are drawn, free for everyone, and licensed under the SIL Open Font License 1.1. No email, no
account, no paid tier. → **[vigilicons.com](https://www.vigilicons.com)**  ·  a written entry per
icon at **[vigilicons.com/words](https://www.vigilicons.com/words)**

All 111 Vigil Icons as SVG, React components and a web component. Stroke-first, rounded corners, drawn on a 24 grid, shipped as a single `currentColor` path per icon so they scale and recolour like text. Free for anything you make — see LICENSE.txt. Drawn by [Keno Vigil](https://thinkkeno.com); the set pairs with the free [Vigil typeface](https://www.vigilfont.com/).

```sh
npm install vigil-icons
```

## React

```jsx
import { Gaslighting, Ghosting, RedFlag } from "vigil-icons";

<Gaslighting size={32} />                 // takes the text colour
<RedFlag color="#FF2D95" title="Red flag" />  // title makes it an accessible image
```

Every icon is a component named after its slug in PascalCase (`couldve-been-an-email` → `CouldveBeenAnEmail`, `six-seven` → `SixSeven`). `icons` is a map from slug to component.

## No framework

```html
<script type="module" src="https://cdn.jsdelivr.net/npm/vigil-icons/web/vigil-icon.js"></script>
<vigil-icon name="ghosting" size="20"></vigil-icon>
```

## Which one

- **React** tree-shakes: import one icon and your bundle carries that one — about 2 KB gzipped, not the set.
- **Plain SVG** is the answer for one icon with no build step: the file, the CDN URL, or the sprite.
- **The web component** carries all 111 paths (about 150 KB gzipped) because there is no build step to shake with. Reach for it when a page wants many icons and no tooling; it warns in the console if a name is misspelt.

## Plain SVG

- Files: `node_modules/vigil-icons/svg/<slug>.svg`
- CDN: `https://cdn.jsdelivr.net/npm/vigil-icons/svg/<slug>.svg`
- Sprite: `sprite.svg` with `<use href="sprite.svg#vi-<slug>">`
- `icons.json`: every icon's number, slug, name and one-line description.

Slugs and descriptions: https://www.vigilicons.com/icons.json

## Other formats

PNG, sticker packs (iMessage, Telegram, WhatsApp) and Slack/Discord emoji zips are on https://www.vigilicons.com/#download.
