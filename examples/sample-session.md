# Sample session (condensed)

**You:** teach me CSS

**Tutor:**
## 🔨 Assessment — Product Card

```
┌──────────────┐
│ [  image  ]  │
│ Title        │
│ [  Button ]  │
└──────────────┘
```

Requirements:
- A card with an image placeholder, a title, and a button
- Make it look decent however you like

Paste when done.

---

**You:** *(pastes HTML + CSS that uses `margin-left: 47px` to center the title and `float` for layout)*

**Tutor:** Here's what your code shows me. You've got colors, borders and hover states down. But the `margin-left: 47px` centering and the floats tell me layout is the gap. Plan for the next hour:

| # | Micro-Project | What it teaches | Est. time |
|---|---|---|---|
| MP1 | Center the card content | flexbox main/cross axis | ~10 min |
| MP2 | Menu grid of 3 cards | flex-wrap + gap | ~12 min |
| MP3 | Sticky nav bar | `position: sticky` | ~10 min |
| MP4 | Mobile layout | media queries | ~15 min |

## ⚡ Concept Flash — Flexbox axes

Think of a flex container as a shelf. `justify-content` slides items *along* the shelf. `align-items` moves them *across* it.

```css
.card { display: flex; flex-direction: column; align-items: center; }
```

Use it any time you'd otherwise reach for a hard-coded margin to center something.

## 🔨 MP1 — Center the card content
Rebuild your card so everything is centered with **no margins used for centering**. Paste when done.

---

**You:** *(pastes code)*

**Tutor:**
**What's correct:** `flex-direction: column` with `align-items: center` is exactly right, and your button now centers at any card width.
**Bug:** `justify-content: center` does nothing here because the card has no fixed height. It only works when there's free space along the main axis.
**Note:** Good instinct reaching for `gap` instead of margins between children.
Move on to MP2.
