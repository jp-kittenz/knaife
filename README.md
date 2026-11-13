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
