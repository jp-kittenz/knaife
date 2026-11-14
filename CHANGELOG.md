# Knaife changelog

Build numbers are shown in the bottom-right corner of the main menu.

## Build 52
- **Gearbox redesigned.**
- **New intro, cut to the boss track.** The music starts on the black screen and the picture follows it:
  - 0:00: black. 0:00.4: a furnace wakes behind one great wheel.
  - 0:03.6: a wall of clockwork ticks in the dark.
  - 0:07.1: the drive chain snaps taut. 0:08: the furnace doors slam open and the engine spins up.
  - 0:09.7 to 0:11.2: on each hit of the snare roll, a pawl clicks the live boss round one tooth while the camera steps out and the RPM readout climbs.
  - 0:11.3: the drop lands on the gameplay framing with no cut. The HUD assembles from shards and the knife rises into place.
- **Boss art:**
  - A machined gunmetal face with lathe rings and heat-tempered colour around the hub.
  - A raised, knurled rim with hex bolts, and chamfered spoke windows.
  - Behind the windows, machinery turns and glows with the bass.
  - An engraved brass hub, and an iris eye whose blades open and close with the music.
  - Teeth lit per flank from the room light, plus a sheen that stays put as the gear turns.
- **Background follows the song, not just the beat:**
  - Quiet sections cool the engine hall to steel blue and slow the machines.
  - Loud sections bring the furnace up, double the gear-train speed and slam every piston on the downbeat.
  - A tach ring around the boss fills with the song's intensity and flashes the redline on drops.
  - Also: foundry windows with light shafts, a flywheel, wall chains, a molten floor channel, grinder spark fans on the hats, embers and steam.
- **Sound variety:** gear hits and ratchet clicks each pick from several recipes.

## Build 51.2
- Water Tanker pipe obstacles redesigned:
  - A lit steel cylinder whose shading follows the room light as the tank turns.
  - A bolted base saddle with a weld bead, a weld seam and a mid collar with hex bolts.
  - A hazard band and a red inline valve wheel.
  - An elbow rising to a bolted end flange, with an open bore of water that pulses with the music.
  - Pipes glow hot during heat cycles. The robot arm carries the matching pipe.

## Build 51.1
- Hits no longer pause the log: the spin hitch and the per-hit freeze are gone, so it keeps spinning through every stick. The jolt, the knife spring-back and the impact ring stay.

## Build 51
- **PixiJS GPU effects layer** (PixiJS 8.6.6, vendored in `assets/`):
  - A full-resolution overlay that shares the game camera draws all hot effects crisp, over the pixel-art world.
  - Effects: spark streaks that cool from white to red, soft glows, lens-flare crosses, impact rings and knife flight trails.
  - Particles come from one texture atlas, one ParticleContainer and a reused pool of 1,500.
  - The layer hides itself when there is nothing to draw and during black-and-white frames. Without WebGL the old canvas effects are used.
- **Punchier feel:**
  - A 45 ms hit-stop on every stick (70 ms in combos).
  - The log jolts on a spring and its spin hitches on each hit.
  - Every knife drives past its seat and springs back.
  - An impact ring pops at the stick point.
- **Crisper everywhere:** higher-resolution rendering in every stage, with lighter dithering and a smoother palette blend.
- **Lit log faces:** the end grain is embossed so ridges catch the light, with a warm key light from the upper left, a cool fill from below and a rim highlight.

## Build 50
- **Water Tanker intro, round two.**
  - **Music:** the boss track now starts on the very first black frame, from its first note. The intro holds on black until the track is actually playing, then stays locked to it.
  - **Upright tanker:** it now stands upright in front of the lit wall, as a backlit silhouette with a rim light. The camera orbits it 360° in 3D, then rises over the top and lands exactly on the gameplay lid.
  - **Tank detail:** hazard bands, rivet rows, a ladder, a sight glass, a KNAIFE WATER plate, an outflow pipe with a valve, and a catwalk rail.
  - **Heavier effects:**
    - The star has god rays, beat rings, a shockwave and sparkles.
    - The gauge slams in, with a turning warning light, steam from the fittings and a shaking needle.
    - The shatter sends out glinting shards, a water jet, sparks and a shockwave, and the pipes crumple.
    - The light flickers on with a hum and dust in the beam.
    - Spotlights land in sequence at the drop.
  - **Cinematic look:** a heavy vignette and film grain.
- **HD mode for this boss:** finer resolution, half the dither, and a smoother palette blend. It drops back to normal resolution outside the boss.
- **More sound variety:**
  - Core sounds now have several takes each, and the same one never plays twice in a row: 4 knife-into-wood impacts, 3 metal impacts on the tanker, 3 throws and 3 knife-on-knife clangs.
  - New intro sounds: star hit, gauge slam, needle rattle, steam jet, glass shatter, pipe implosion, lamp hum, spotlights, HUD shards assembling, and the knife rising.
  - New robot-arm sounds: servo whirr, punch and welding.

## Build 49
- **Water Tanker rebuilt.**
  - **Intro, cut to the track:** every beat lands on a hit measured from the music file, and the picture follows the song's real playback position.
    - 0:01 a rotating gold star on the first hit.
    - 0:04 the pressure gauge slams in, with shadowed pipes drifting at three depths.
    - 0:06 the needle shakes on the last dial.
    - 0:08 the glass bursts and the pipes implode.
    - 0:09 a dark pan along the pipe to its elbow.
    - 0:12 the light comes on: the tanker in silhouette on the wall.
    - 0:13 a full 3D orbit, then the camera swings over the top and lands exactly on the gameplay view (no cut).
    - 0:15.65 (the drop) spotlights snap on, the HUD assembles from flying shards with a flash, and the knife rises into the lane.
  - **Boss art, seen from overhead:** a caution-striped lid, a big pressure gauge, portholes, a hatch and a KNAIFE WATER stencil, turning inside a collar held by fixed hazard-striped mounts, with a slow leak dripping off the left mount.
  - **Pipe obstacles are built live:**
    - A pipe punches a hole in the tank.
    - A robot arm places the pipe and welds it.
    - It brings the base flange and welds again.
    - Pipes block once they are placed.
  - **New overhead background**, five layers deep:
    - The plant floor, with background tanks, control platforms, and hard-hatted workers running around the tanks.
    - Red, yellow and green pipe networks at increasing depth.
    - The boss.
    - A blurred purple foreground.
    - It is procedurally generated, scrolls right with parallax, and is full of valves, steam vents, outflows, lamps and alert beacons.
  - **The background follows the song, not just the tempo:**
    - Floodlights bang on with beat 1 and off with beat 2.
    - Everything runs faster and harder as the music builds.
    - Alert beacons spin up ahead of build-ups.
    - The lights strobe on the drops.
    - A pressure ring goes out every bar.
    - This is driven by a per-beat map of the track's energy, bass and highs, plus a live analyser on the music.
- Failure frames are back to black and white.

## Build 48
- **Redesign pass on look, feel and sound** (theme kept: the sawmill, the pixel palette, the red accents).
- **Lighting and rendering**:
  - A warm work light falls on the log, with dust turning in the beam.
  - The mill floor runs away beneath it in plank seams and sawdust.
  - New GPU bloom: only genuinely hot things glow (sparks, fire, charge, neon), and the glow is dithered into the same palette as everything else.
  - Vignette.
  - Life-loss and impact frames are now red and black instead of a white screen.
- **Effects**:
  - Sparks are streaks that cool from white to red.
  - Contact flares appear where knives stick.
  - Screen shake now uses smooth trauma with a slight roll, so small hits stay subtle and big ones snap.
  - The light swells on heavy hits.
- **Knife**: a breathing bob, a glint running down the blade, and a contact shadow on the floor.
- **HUD redesign**:
  - Score plate with a count-up and BEST, with hearts under it.
  - A stage track with progress line and boss diamond.
  - Log-type info as a fitted chip (it no longer runs into the hearts).
  - Apples by the mute button.
  - A knife magazine rack.
- **Sound engine**:
  - Every sound varies slightly in pitch and stereo position.
  - New damped stereo reverb with early reflections.
  - Compressor plus limiter.
  - Music ducks under heavy hits.
  - Lighter on CPU, since noise is no longer generated per sound.
  - New throw, stick, knife-on-knife clang and combo sounds.

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
