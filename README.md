# 100% Pure CSS Slot Machines

A fully functional slot machine built with **pure CSS**.

- ✅ 10 lines of HTML (just an empty body)
- ✅ 872 lines of CSS
- ✅ **0 lines of JavaScript**

Submitted to [Gamedev.js Jam 2026](https://itch.io/jam/gamedevjs-2026) — theme: **Machines**.

## Features

- 3D cylindrical reels with inertial stops
- 6-step bet long-press cycle (1, 2, 3, 5, 10, 40)
- 5-line win detection
- BONUS / FREE modes with state hoisting in pure CSS
- Live clock, paytable, status panel, scrolling footer
- Metal-textured backgrounds (silver / gold mode switch)

## Theme: Machines

- The work itself is *Slot Machines* (the plural is intentional).
- BONUS mode triggers a "MACHINES" theme: symbols turn mechanical (🔩🔧⚙️🦾🤖🎰).
- Internally, 76 virtual components are wired together as a single machine.
- The CSS engine itself is used as a computational machine.

## Browser Support

Requires the latest **Chrome / Edge / Opera**. Other browsers may not render correctly. Designed for desktop.

Uses cutting-edge CSS features:

- `@function` and `if()` with `style()` queries
- `animation-timeline: scroll()` for state register
- `::column` + `::scroll-marker` as virtual components
- `@property` for typed custom properties

## Architecture Highlights

- **Scrollbar as memory**: a 6-bit state register encoded in scrollbar position
- **State Hoisting**: all state lives at `html` / `body`, components are pure render
- **3-layer naming**: `class` (identity) / `role` (function) / `element` (HTML-ish type)
- **Frame-precise interaction**: 75ms `pointer-events` discrete transition syncs with 50ms-per-step keyframes

## How to Play

1. Open `index.html` in Chrome / Edge / Opera (latest).
2. Wait for loading.
3. Long-press "bet" to set wager.
4. Press "play" to spin.
5. Hit each "stop!!" to halt the reels.
6. Match 3 symbols on any of 5 lines to win.

## License

MIT
