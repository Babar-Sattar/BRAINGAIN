# BrainGain homepage — Option A (dark)

Mobile-first prototype. Content order is Babar's; this file is the visual
direction.

## Why dark

A light-ground version was built and rejected. BrainGain's assets are a
dark-brand set: the products are black, the logo is drawn light and only works
on a dark band, and the cyan is a neon that goes weak on white. Dark isn't a
preference here, it's what the existing assets support. Both photo sets are in
`images/` so the light option can be reconstructed if anyone wants to see it.

## Corrections made on 28 September 2026

Three claims on the page were wrong. All three were checked against
braingain.fit and its published policies that day:

| Was | Now | Source |
|---|---|---|
| Free delivery | **Free UK delivery** | homepage promise band |
| 3-year warranty | **2-year warranty** | homepage promise band ("Elite 2-Year Warranty") |
| 30-day returns | **14-day returns** | /policies/refund-policy, "We have a 14-day return policy" |

The 3-year figure is the **EU** site's. This prototype prices in pounds, so it
is the UK page and takes the UK terms. Worth confirming with Adil which market
this is for, because the promises change with it.

## Other changes this round

- Hero tightened. The CTA now clears the fold on a 375px iPhone SE, a 390px
  iPhone 14 and a 430px iPhone Pro Max. It was landing on the fold line.
- Subhead restored: "Serious about training, short on space?" It is the
  cheapest answer to "is this for me?" and it had been lost.
- "As seen in" heading added to the press rail.

## Interactive

- **Press rail and review rail** drift right to left, seamless loop, pause on
  hover and on keyboard focus. Both are real scroll containers, so they can be
  swiped on touch and click-dragged on desktop. Under
  `prefers-reduced-motion` they stop drifting and stay swipeable.
- **Best sellers** and **Our products** carousels: chevrons, dots, swipe,
  arrow keys. The product name below Our products updates with the slide.
- **Scroll reveal**, disabled under `prefers-reduced-motion`.

## Assets

```
index.html
images/
  product-black.jpg / product-chrome.jpg    best sellers
  cat-*.jpg                                 our products, studio shots
  alt-room-*.jpg                            the in-room set, unused here
  founders.jpg                              NOT INCLUDED
```

`images/founders.jpg` is still missing from this folder. Copy it from the v2
prototype. Until then the story section shows a striped placeholder.

The five press mastheads are hot-linked from the Shopify CDN. If one fails the
page prints the publication name as text. On a dark ground the three with a
white background baked in (Runner's World, GQ, Women's Health) are inverted;
the two with real transparency (Men's Fitness, T3) are forced to white.

## Known, not fixed

- Nothing on the page proves the headline. The before/after and the weight
  slider both moved to the PDP, so "a full rack in one dumbbell" is asserted
  and never demonstrated. The hero video is meant to carry it.
- "Best sellers" is plural and shows one product in two colours.
- Best sellers and Our products are the same component doing different jobs.
- Trustpilot appears twice: the evidence bar and the 4.7 block.
- Section gaps double to 144px where two sections meet.

## Not verified

Price (£169.99 / £299.99), product title and the 469 review count were read
from the live UK store on 28 September 2026. Trustpilot: 4.7 "Excellent",
2,087 reviews, same date. The press quotes are transcribed from the Figma and
have not been checked against the original articles.
