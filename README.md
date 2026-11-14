# Knaife

A knife-throwing web game. Open `index.html` in a browser.

- Tap, click, Space/Enter/Up to throw; M to mute
- Stick every knife in the spinning log; hitting a stuck knife costs one of 3 lives (impact frame, black & white, knife shatters); losing the last one shatters the whole screen into a black & white game-over; retry rebuilds the screen from the shards, flashes, flips the lights on and smashes a START sign
- Slice apples for +2; every 5th stage is a boss log with tricky spin
- Ability (button bottom-right, or E / Shift): arms the next knife for a slow-motion double-damage throw.
  Hitting a stuck knife destroys it (1 damage, no life lost); a killing blow slices the log in half.
  Recharges after 4 successful hits.
- Grazing the side of a stuck knife ricochets your knife away (no life lost, knife refunded), tilts the stuck knife, and stuns you for 2s.
- Log types (random each stage from stage 2): branched (plain, swirly, burning, beehive, wired, chained, bird), weak-spot holes (x2),
  overgrown bushes (apples or hidden knives), moss armour, segmented armour plates, hungry tree hollow (swallows knives, burps one back every 3rd), an unbreakable sawmill (timer).
  The knife ability has its own interaction with each type (see `KNIFE_ABILITIES` in index.html).
- Main menu: 3D floating PLAY / STORE / ENCYCLOPEDIA slabs in a haunted sawmill corridor. The store shows the equipped blade
  (drag to spin) and banked apples; the encyclopedia covers every log type, branch, boss and mechanic with live demos.
- Knife: REGULAR KNIFE, ability STRONG THROW (ACTIVE). The store has KNIFE and ABILITY tabs.
- Music: `assets/music.mp3` (supplied by the project owner) loops from the entry screen; slow-mo lowers its pitch and impacts muffle it.
- Knives (equip in the store): Regular Knife (Strong Throw), Precision Dagger (Marker), Carving Knife (Knife with a Knife),
  Conductive Knife (Chain Reaction + passive Overvolt), Kitchen Knife (Cook + passive Get the Bird). Items appear in a tray above the ability button (keys 1 / 2).
- Boss (stage 5, one of four picked at random): WATER TANKER — knives forced out leave leaks, a 60s flood clock, heat cycles, a deadly pipe, crane intro and explosive splash finish.
- Boss (stage 5, alternative): GEARBOX — 20 hits, ratcheting spin, pinion gears on the rim cost a heart; machinery set (drive gears, beacons, vents, RPM holo); phase 2 blows its plates off and bowls sprocket shots down the lane; summons two gears and swaps itself for a decoy while a drive chain blocks the lane. Crack 3 links or hit the red master link to snap it (jams the boss, -2 HP); yellow sleeves stun; too slow and it repairs. Blueprint-to-machinery intro with paint splashes and its own track.
- Boss (stage 5, alternative): MONSTER TIRE — rubber layer (first hit bounces and leaves a chalk mark, second hit on the mark punctures; 10 punctures, then knock a stuck knife out to deflate it), then 20 hits on bare steel. 4s burnout every 7s, fold-out blades, knives thrown off, loose lug nuts in the lane; night-road/burnout intro.
- Boss (stage 5, alternative): HORNET'S NEST — starts disguised as a branched log; breaking its beehive triggers the boss. Orbiting wasps sting (4s stun, spin flips), infested spots/knives jam the ability 40s, a breach every 8 hits (x2 spot, more wasps, wasps on the screen), then the queen rebuilds it to 10 HP and defends it with five moves.

## Redesign (build 38)
- Parallax mill hall (far windows, idle blades, chains, foreground rigging and sawdust) driven by idle sway, mouse / device tilt and impacts; the log has real depth that follows it.
- New log types: BLACKOUT, POWDER KEG, FROSTBITE. New perches: crow, woodpecker, owl. Every type has its own face art and ambience.
- Display font with per-letter banner slams; rapid combos, close calls, slow-motion finisher, flawless bonus; saws slide in and spin down / retract.
- Marker, Carve, Chain and Cook each react to every log type (see the encyclopedia, which follows the equipped knife).
- Faster pacing and richer sound.

## Build 39
- Hornet's Nest has its own music: the nest theme (Flamewall cut, loops bars 33.2s-110.0s on a crossfaded seam) and a queen theme (loops 0.12s-19.32s). The hive break tape-stops the stage music and slams into the nest theme; the queen's hatch tape-stops it, cuts to silence and slams into the queen theme.
- 28 ability interactions per knife (11 log types, 5 branch kinds, 4 birds, apples, hidden knives, 4 named bosses, the queen, classic bosses), called out in an on-screen feed and listed per knife in the encyclopedia.

## Build 44
- Every log feature redrawn and reanimated: shaded tapered branches with flipping leaves, layered flames that rise with the screen, a steel coil spring, a swinging beehive that drips honey, a frayed sparking cable, a sagging padlocked chain, layered swaying bushes, scalloped moss with strands and dew, tunnel weak spots with beating cores and a walking beetle, a hollow with brow, eyes, jaw, tongue and breath, bevelled armour with a sweeping sheen, a motion-blurred saw.
- New log types: LODESTONE (magnetic pulses bunch knives, poles repel), BRAMBLE (orbiting thorn vines snag), FUNGAL LOG (mushrooms x2 + spore haze), RUNESTONE (hit the lit rune for x2 and charge).
- 32 ability interactions per knife.

## Build 45
- New log types: SPIRALWOOD (three spiral tracks shift every 3 hits, carrying their knives), RESINWOOD (resin holds knives for 0 damage; a second hit cracks the patch), PETRIFIED LOG (stone ricochets harmlessly, hit the wooden seams; stone crumbles after 3 hits), EMBERCORE (drifting glowing cracks flare when hit and the glare hides nearby knives), RINGWOOD (three coloured rings; every 3 hits one rises and its knives slide outward).
- 37 ability interactions per knife.
