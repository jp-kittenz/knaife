# Build 48 redesign: evidence

Skills used (loaded from `.claude/skills`): threejs-game-director, threejs-aaa-graphics-builder (visual-scorecard.md), threejs-game-ui-designer (ui-patterns.md), threejs-gameplay-systems (game-feel.md), threejs-webaudio-generative-soundtrack, threejs-bloom. The Three.js scaffolding does not apply (Knaife is a 2D canvas + WebGL post game); their quality bars, feel recipes, UI rules, audio bus and bloom ordering were applied.

## Scorecard (phone 412x915 + desktop 1280x720, active play)
Genre mapping: hero = knife + log, obstacles = stuck knives and log hazards, rewards = apples/branches/pickups.

| Category | Before | After | Evidence |
|---|---|---|---|
| Art direction | 2 | 2.5 | warm mill key light, plank floor, red/black impact frames match the red accent identity |
| Hero (knife/log) | 2 | 2.5 | blade glint, idle bob, contact shadow, stick flare; log lit by the key light |
| Obstacles | 2 | 2 | unchanged forms |
| Rewards | 1.5 | 2 | saturated pickups now bloom; contact flares |
| World | 1.5 | 2.5 | perspective mill floor fills the lower half, dust in the light beam, full-width on desktop |
| Materials | 2 | 2 | unchanged |
| Lighting/render | 1.5 | 2.5 | selective bloom before palette quantize, vignette, light pool, bloom swell on heavy hits |
| VFX/motion | 2 | 2.5 | velocity-streak sparks cooling white→red, trauma² shake with roll, red/black impact frames (no white) |
| UI/HUD | 1.5 | 2.5 | clustered HUD, stage track, fitted type chip, magazine rack; overlap with hearts fixed |
| Performance | 2 | 2 | Pixel 7 emulation (SwiftShader, CPU): 48-61 fps steady (first entry dips to ~40 while sprites bake) |
| **Average** | **1.85** | **2.3** | automatic fails fixed: HUD overlap, white full-screen flashes |

## Checks run
- Regression suite: t19, t30, t32, t40, t50, t60, t61, t70 (5 knives x 38 interactions, 0 fails), t73, t80, t96, t97, t110: all pass.
- Audio: all 145 sfx functions called on the new engine with no errors; context running; ducking engaged.
- Captures: baseline and after, phone and desktop (menu, play, flight, impact, life loss, boss), and a 30 ms throw sequence.
