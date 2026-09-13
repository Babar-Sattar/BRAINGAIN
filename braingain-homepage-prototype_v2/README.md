# BrainGain EU — homepage concept

Interactive mobile-first prototype of the redesigned BrainGain EU homepage.
Design by Babar Sattar. This is a prototype for client review, not production code.

## Run it

Open `index.html` in a browser, or drop the whole folder into a GitHub repo and
turn on GitHub Pages (Settings → Pages → Deploy from branch → `main` / `root`).

Keep the folder structure — `index.html` expects `images/` next to it.

```
index.html
images/
  slider-1.jpg … slider-5.jpg   product at five plate configurations
  room-before.jpg               living room with a full dumbbell rack
  room-after.jpg                same room, one pair of SmartBells
  founders.jpg                  BrainGain founders, Dil and Kareem
```

## What's interactive

- **Before / after flipbook** — tap the image, use the Before/After control, or
  focus it and press Enter. Crossfades. Full-bleed, no side gutters. The
  Before/After control sits on the image and doubles as the state label.
- **Weight slider** — five stops. Drag or use arrow keys. Changes the product
  image, the kg readout and the zone label. Starts at stop 3 (20 kg).
- **Reviews conveyor** — eight real reviews from the live EU store, scrolling
  continuously over a photo background. Pauses on hover and on keyboard focus.
  Under `prefers-reduced-motion` it becomes a normal swipeable row with no
  animation and no duplicated cards.
- **Scroll reveal** — sections fade up on entry. Disabled under
  `prefers-reduced-motion`.

## Placeholders and unverified content

- **Hero video** — a styled placeholder. The design assumes the top 25% and
  bottom 25% of the footage stay visually quiet so the headline and CTA stay
  legible. That's a constraint on what can be shot.
- **Before / after labels** are HTML, not baked into the image files, so the
  German site can render VORHER / NACHHER without re-exporting artwork.
- **Weight values on the slider** — plausible placeholders mapped to the five
  supplied product shots. Confirm the real figure per configuration.
- **Product images on the best-seller cards** — hot-linked from the live
  Shopify CDN. Download them into `images/` if you want the page fully
  self-contained.
- **Prices and review counts** — read from the live EU store. No invented
  "was" prices.

## Surface rhythm

White sections were stacking into one slab. Three changes break it up:
the before/after image runs full-bleed, the product stage sits on a hairline
card rather than a grey one, and best sellers sits on `--light-2`. The reviews
section then lands as a dark photographic break before the story.
