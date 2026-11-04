# Pizza Dash — Store Submission Materials

## Short description (CrazyGames / GameDistribution / itch.io)

Ride your scooter through a neon night city. Grab pizzas at the pizzeria
and race them to the marked doorstep before the timer melts the cheese —
every late order costs a star. One bike, one pizza, zero mercy.

## Details

- Genre: Driving / Arcade / Casual
- Controls: Keyboard — ↑/W gas, ↓/S brake & reverse, ←→/A D steer, M mute.
  Mobile: on-screen touch pads (steer left/right, gas, brake).
- Features: procedural night city with guaranteed-connected streets,
  30s+ timed deliveries scaled by route distance, one-order-at-a-time flow,
  +30 pts per on-time drop, 5-star rating from average delivery time
  (late orders void and cost a star), BFS pathfinding arrow with distance,
  60s Sprint and 3-Min Rush modes, best score & most deliveries saved
  locally, mute toggle. Crashing into buildings just slows you down —
  no damage, pure arcade.
- Visuals: warm-lit windows, street-lamp halos, headlight cone, thermal
  pizza box, door bubbles, coin float text. All drawn in canvas, no assets.
- Audio: fully synthesized WebAudio — engine hum that follows your speed,
  pickup chime, doorbell ding + coin arpeggio, timeout buzz, countdown ticks.
- Tech: single-file HTML5 (Vanilla JS + Canvas 2D + WebAudio). No frameworks,
  no external assets, works offline once loaded.

## Tags
driving, arcade, pizza, delivery, city, night, casual, time-management, single-file

## CrazyGames submission checklist
- [x] Self-contained index.html (SDK loads only on crazygames domains)
- [x] gameplayStart / gameplayStop / loadingStart / loadingStop / happytime events wired
- [x] Responsive canvas, portrait- and landscape-friendly, touch + keyboard
- [x] No external links inside gameplay, no analytics
- [ ] Cover art 16:9 (generate from gameplay screenshot)

## GameDistribution
- Upload `pizza-deliver-gd.zip` (contains only index.html).
- SDK script (sdk.gamedistribution.com/v2/main.min.js) loads automatically on
  gamedistribution / gd.games domains via the domain-guard loader.

## itch.io
- Upload `pizza-deliver-itch.zip`, mark "This file is playable in browser",
  entry file: index.html, kind: html. Any viewport works (responsive canvas);
  recommended embed 960×640.
- Pricing: $0 (donations optional)

## Live
- https://shuangyueliao.github.io/pizza-deliver/
