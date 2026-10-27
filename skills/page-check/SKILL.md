---
name: page-check
description: Checks a web page, landing page, booking form or app screen against a phone-first standard with numbers - no sideways scroll, 44 px tap targets, 16 px text, nothing clipped or covered by a sticky bar, no dead empty boxes, copy that fits in English and Spanish, step text one action per sentence, and money shown clearly. Use before shipping or after editing any page, or when the user says "check this page", "it looks off on my phone", "review the layout" or "is this ready".
license: MIT
metadata:
  author: Isla Tech LLC
  version: "1.0"
---

# Page check

Most customers see your page on a phone, often in the sun, often in their second language.
Check every page against these numbers before it ships. Report each failure with the element, the screen size and the fix.

## 1. Sizes to check

Check at least: **360 × 740** (small Android), **390 × 844** (the reference phone), **768 × 1024** (tablet),
**1440 × 900** (desktop). Phone first.
- No sideways page scroll at any size.
- Content never touches the screen edge: 16 px side gutter on phones, 24 px on tablets.

## 2. Controls

- **Tap targets at least 44 × 44 px** on touch screens (48 is better), at least 8 px apart.
- **Form fields 44 to 48 px tall, text 16 px** (smaller text makes iPhones zoom in).
- **Labels sit 4 to 6 px above their field.** A placeholder is a hint, never the only label.
- **Short values share a row:** date + guests, first + last name. A 1 to 3 character value never gets a full-width box.
- **Numbers are steppers** (`[ − ] 2 [ + ]`). **Up to 8 options are chips,** not a dropdown.
- **One main action per screen,** full width on phones (max 480 px), 48 px tall.
- **No grey browser-default buttons or boxes.** Every control wears the page's style.

## 3. Nothing covers anything

- A sticky top bar or bottom bar reserves its own space. Scrolled to the very bottom, the last line and the last
  button are fully visible above the bar.
- A floating chat or help bubble never sits on a button or a form field.
- An open menu covers the whole screen with a backdrop, or nothing.
- Sticky top bar at most 64 px tall on phones.

## 4. Text

- **Nothing essential is cut off:** names, prices, dates, button labels, headings. No "…" on those.
- **Copy fits in English and Spanish.** Spanish runs about 25% longer: if "Book" fits, check "Reservar" fits.
- **Body text 16 px on phones,** nothing under 11 px anywhere.
- **Pills and small labels stay on one line.** If a label wraps, shorten it.
- **Labels give the customer's reason** ("Popular with riders"), not your internal metric ("60 taps").

## 5. Steps and instructions

For how-to text (check-in, pick-up, returns, safety):
- One action per sentence. A step starts with its verb: "Lock the bike to the rack."
- A step is 20 words or fewer (25 in Spanish).
- Say who does it: "We charge the deposit when you book."
- A warning comes **before** the step it applies to.
- "Must" and "do not", never "should" or "might".
- Three or more steps are numbered.

## 6. Images

- The subject (the product, the face) is inside the frame at every size. Pick the crop on purpose.
- **Product photos are never cropped:** show the whole product.
- One aspect ratio per grid. Never stretched. Every image has `alt` text.
- Text on a photo gets a shadow or a plate so it reads.

## 7. Empty space

- A box's height comes from its content. No fixed tall cards with three lines inside.
- A card whose content fills under 25% of it is a dead box: shrink it or fill it.
- Cards in a row line up their buttons on one line.
- Space between sections is even (32 or 48 px). Dead space is space nobody decided.

## 8. Money (owner and admin screens)

- A negative number or money going out shows in parentheses: `($743)`, never `-$743`.
- The label says which way the money goes: "Spent this month", "Revenue". Never a bare "This month" over a dollar figure.

## Report format

```
PASS  360×740  no sideways scroll
FAIL  390×844  "Reservar ahora" button is 36 px tall → make it 48 px
FAIL  390×844  sticky Book bar covers the last FAQ answer → add bottom padding = bar height + 16 px
WARN  768×1024 3 cards then 1 alone → use 2 + 2
```

End with the count of fails and the one fix that matters most.
