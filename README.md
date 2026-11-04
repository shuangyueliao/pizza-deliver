# Pizza Dash

A free single-file HTML5 pizza delivery driving game. Ride your scooter
through a procedurally generated night city, grab pizzas at the pizzeria
and race them to highlighted doorsteps before the timer melts the cheese.

**Play:** https://shuangyueliao.github.io/pizza-deliver/

## How to play

- An order marker appears over the pizzeria — follow the gold pathfinding
  arrow, ride into the pickup ring to load the pizza into your thermal box.
- Deliver to the pulsing house marker (exclamation bubble at the door).
  On time: +30 pts. Too late: the order is voided and you lose a star.
- Each order gives 30 seconds, plus extra time for longer routes.
- One pizza at a time — deliver before the next pickup appears.
- Buildings don't hurt you; they just slow you down (arcade bump).
- **5-star rating** is earned from your average delivery time; every
  late/voided order knocks one star off.
- **60s SPRINT** and **3-MIN RUSH** modes; best score and most deliveries
  per mode are saved in localStorage.

## Features

- Procedural night city: connected street grid (pruned-edge generation with
  a connectivity guarantee), warm-lit windows, street-lamp halos, lane dashes.
- Drift-lite scooter physics: throttle, brake/reverse, inertia with lateral
  grip; wall bumps scrub speed instead of ending the run; anti-wedge nudge
  keeps you moving.
- BFS pathfinding arrow with live distance readout points along real roads.
- Headlight cone, brake light, pizza thermal box, door bubbles, +30 coin
  floats, delivery ding-dong, countdown ticks, engine hum that follows speed.
- Mobile touch pads + desktop keyboard (↑/W gas, ↓/S brake, ←→/A D steer,
  M mute), responsive canvas with camera follow.
- Start menu and settlement screen (deliveries / on-time rate / avg time /
  star rating), mute toggle persisted.

## Tech

- One `index.html` (~44 KB), zero external assets — no CDN, images, or fonts.
- Vanilla JavaScript + Canvas 2D + WebAudio. No frameworks, no tracking,
  no external links.
- Portal SDKs load only on matching domains (CrazyGames / GameDistribution);
  the file runs standalone with no SDK calls.

## Files

- `index.html` — the whole game
- `.nojekyll` — bypasses GitHub Pages Jekyll processing
- `store/` — submission materials (description, GameDistribution zip, itch.io zip)

## License

MIT
