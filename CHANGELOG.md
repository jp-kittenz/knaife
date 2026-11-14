# Knaife changelog

Build numbers are shown in the bottom-right corner of the main menu.

## Build 47
- **The Wire Clump, redesigned**: it is now a real 3D ball of cable. Two dozen insulated wires are wound like a ball of yarn, depth-sorted and lit, and it wobbles as it spins.
  - A charged core glows through the gaps and swells with the beat and the voltage.
  - Current crawls along the strands, and cut ends spark.
  - Braids are thick twisted copper-and-steel rope with brass ferrules.
  - Heavy ribbed conduits run to junction boxes on the walls.
  - The wire cutters are giant bolt cutters with red grips and a countdown.
  - Ground wires hang with a hazard tag.
- **The Wire Clump, nerfed**:
  - 22 hits (was 26).
  - Longer safe spells and shorter dangerous ones. Only DANGEROUS counts now, not RISING.
  - Bare wire costs 9% stability (was 14%), and braid hits restore 3%.
  - Cutters snip for 12% (was 18%), arrive less often and give you longer to smash them.
  - Fewer, shorter-lived ground wires, a 2s stun, rarer random cable snaps.
- **Boss backgrounds rebuilt, packed with energy and on theme**:
  - Water Tanker: a flooded pump station with sloshing tank gauges, racing flow arrows and swells.
  - Gearbox: an engine room with gears stepping a tooth per beat, pistons hammering in turn, a conveyor and furnace embers.
  - Monster Tire: a midnight arena with a striped synthwave sun, a bouncing crowd, chasing floodlights, a neon grid floor, fireworks and flame jets.
  - Hornet's Nest: light washing across the comb, dripping honey and rivers of hornets. The Queen gets crimson comb and a turning crown of spikes.
  - Wire Clump: a storm over pylons, live lines, Tesla coils firing on the beat, sky lightning every bar and a circuit floor.
- **Every boss intro reworked as a slow cinematic**: four long takes that fade in and out of black, slow camera moves, captions that wipe in, then the arena light comes up as the boss is lowered, rises, rolls or swings in, and the title rises letter by letter.

## Build 46
- New stage-5 boss: **The Wire Clump**, with its own music.
  - Braided spots are safe. Bare wire deals x3 damage but drains **Stability**, and at 0 the clump explodes and ends the run.
  - A **voltmeter** shows SAFE / RISING / DANGEROUS. At dangerous voltage, touching the clump costs a heart, and stuck knives glow, then explode or melt.
  - Arcs and sparks drop **ground wires** that electrocute.
  - From phase 2, big **wire cutters** must be smashed before they snip a cable.
  - Snapped cables cause a 5s **special blackout**: red alarm beams only, the voltmeter dies, ground wires glow to show the voltage, and workers run past the lit window.
  - Comes with a cinematic intro, an overload death and a meltdown game over.
- Every boss now has its own beat-synced background that pulses with its music: sonar and bubbles for the Tanker, ticking gears and pistons for the Gearbox, a synthwave road for the Tire, flashing honeycomb for the Nest (red with a crown for the Queen), and circuit traces with an oscilloscope for the Wire Clump.
- **Admin panel** (gear button, bottom-left; pauses the game):
  - Pick the next log type and the next boss.
  - Jump to the next stage or straight to the boss.
  - Refill hearts, charge the ability, or turn on god mode.
- Each knife now has 38 ability interactions (new: the Wire Clump).

## Build 45
- New log types: **Spiralwood** (three spiral tracks shift every 3 hits, carrying their knives), **Resinwood** (resin holds a knife for 0 damage, a second hit cracks the patch), **Petrified Log** (stone ricochets harmlessly, only wooden seams take knives, stone crumbles after 3 hits), **Embercore** (drifting cracks flare when hit and the glare hides nearby knives), **Ringwood** (three coloured rings, one rises every 3 hits and its knives slide outward).
- Every knife now has 37 ability interactions.

## Build 44
- Every log feature redrawn and reanimated: shaded branches with flipping leaves, flames that rise upward, steel coil spring, swinging beehive with honey, sparking frayed cable, padlocked swinging chain, layered bushes, scalloped moss with strands and dew, tunnel weak spots with beating cores and a beetle, a hollow with brow, eyes, jaw, tongue and breath, bevelled armour with a moving sheen, motion-blurred saw.
- New log types: **Lodestone** (magnetic pulses bunch knives, poles repel), **Bramble** (orbiting thorn vines snag and stun), **Fungal Log** (mushrooms deal x2 but fill the screen with spores), **Runestone** (hit the lit rune for x2 and ability charge).

## Build 43
- Kitchen Knife gains a second passive, **Bird's Heart**: bird perches turn up on about half of all stages (up from ~3%).

## Build 42
- Regular, Carving and Conductive knives all fly as cinematic power throws and never cost a heart.
- Each has its own outcome for: clean hit, final blow, hitting a knife, grazing a knife, final blow + knife, final blow + graze, cutting through a branch, slicing an apple.
- New lightning everywhere: branching, flickering bolts with glow, forks and travelling pulses.
- Title beats for the Dagger (Target Marked, Bullseye) and Kitchen Knife (Bon Appetit).
- Fix: a final-blow Strong Throw on the Hornet's Nest skipped the queen.

## Build 41
- Every ability interaction plays its own animated set piece at the spot it affects, with a slow-motion beat, camera punch, sound and title.

## Build 40
- Fix: boss music could go silent on phones after playing a few bosses (decoded tracks are now freed once they fade out).

## Build 39
- Hornet's Nest gets its own music: a nest theme and a queen theme, both looping seamlessly, with tape-stop and slam transitions.
- 28 ability interactions per knife, shown in an on-screen feed and the encyclopedia.

## Build 38
- Major redesign: parallax mill hall, 3D log, display font with slamming titles, faster pace, richer sound.
- New log types: **Blackout**, **Powder Keg**, **Frostbite**. New birds: crow, woodpecker, owl.
- Rapid combos, close calls, a slow-motion final hit, flawless bonus; saws slide in and spin down.
- Every ability reacts to every log type. Encyclopedia expanded.

## Build 37
- New stage-5 boss: **Hornet's Nest** (disguised as a branched log, orbiting wasps, infestation, breaches, queen phase with five moves).
- Monster Tire gets its own music.

## Build 36
- New stage-5 boss: **Monster Tire** (rubber and steel layers, burnouts, deflate cutscene, cinematic intro).

## Builds 34-35
- Fix: the white wash over boss intros (the between-stages light flash never faded while an intro froze game time).
- Build number shown on the menu.

## Earlier
- Gearbox boss with gear swaps, breakable drive chain, phase 2 and its own music; the stage-5 boss is picked at random.
- Water Tanker boss with leaks, flood clock, heat cycles, phases and a shot-by-shot cinematic intro.
- 3D main menu, store and encyclopedia; five knives with active and passive abilities.
- Log types with branches, hazards and per-ability interactions; procedural wood textures.
- Pixel-art look with a WebGL palette shader; three lives with impact, shatter and retry sequences.
