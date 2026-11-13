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
- Boss (stage 5, randomly the Tanker or the Gearbox): WATER TANKER — knives forced out leave leaks, a 60s flood clock, heat cycles, a deadly pipe, crane intro and explosive splash finish.
- Boss (stage 5, alternative): GEARBOX — 20 hits, ratcheting spin, pinion gears on the rim cost a heart; machinery set (drive gears, beacons, vents, RPM holo); phase 2 blows its plates off and bowls sprocket shots down the lane; summons two gears and swaps itself for a decoy while a drive chain blocks the lane. Crack 3 links or hit the red master link to snap it (jams the boss, -2 HP); yellow sleeves stun; too slow and it repairs. Blueprint-to-machinery intro with paint splashes and its own track.
