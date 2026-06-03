# imnotaranger Deadeye Repair Report

Source: public poe.ninja character model for `imnotaranger`, account `nega_tive#4060`, Runes of Aldur.

Snapshot used:

- poe.ninja profile: <https://poe.ninja/poe2/profile/nega_tive-4060/runesofaldur/character/imnotaranger>
- Last checked by poe.ninja: `2026-06-03T02:44:03Z`
- Level 68 `Deadeye`
- Main damage shell: `Ice Shot`, `Tornado Shot`, `Snipe`, `Freezing Mark`
- Displayed DPS: `Ice Shot 9375`, `Tornado Shot 4559`, `Snipe 2799`
- Life: `1536`
- Energy Shield: `272`
- Mana: `530`
- Spirit: `139`
- Movement speed: `128%`
- Resistances: Fire `43`, Cold `38`, Lightning `70`, Chaos `0`
- Lowest maximum hit taken: `1672` chaos
- Physical maximum hit taken: `1900`

This report only uses the public poe.ninja snapshot. It does not include map footage, death logs, private stash state, or market budget.

## Short Verdict

This character is not broken because the skill idea is wrong. The bow cold projectile direction is understandable:

```text
1 projectile bow
Ice Shot clear
Tornado Shot coverage
Snipe single-target attempt
Freezing Mark / Herald of Ice / Combat Frenzy utility
Polcirkeln for chill -> shatter conversion
```

The repair problem is much simpler:

```text
The offense is trying to map,
but the defensive floor is still campaign/early-map level.
```

At level 68, fire and cold resistance are not capped, chaos resistance is zero, and both chaos and physical max-hit are under `2000`. That means ordinary mapping can feel random: some packs explode, but bad rares, ground effects, chaos hits, or physical spikes can delete the character before the bow engine gets to play.

The first repair is not a luxury bow. The first repair is capping resistances while keeping enough life and damage to continue progressing.

## What Is Working

### Bow

The bow is good enough for the current stage:

- `+1 to Level of all Projectile Skills`
- added physical and fire damage
- increased elemental damage with attacks
- cold rune damage
- mana leech from physical damage
- extra dexterity

This is not an emergency slot. A better bow will help later, but buying the bow first would leave the same death pattern in place.

### Body Armour

The body armour is one of the better pieces:

- `+198 maximum Life`
- fire and cold resistance
- energy shield
- life regeneration

Keep this until a replacement clearly improves life plus resistance.

### Helmet and Belt

The helmet and belt both have strong life:

- Helmet: `+165 maximum Life`
- Belt: `+158 maximum Life`, 3 charm slots

These are doing real work. They can be improved later, but they are not the first slots to throw away.

### Cold Projectile Identity

The skill package is coherent enough:

- `Ice Shot` for main clear
- `Tornado Shot` for screen coverage
- `Snipe` for aimed burst
- `Freezing Mark`
- `Herald of Ice`
- `Combat Frenzy`
- `Wind Dancer`

This is a playable identity. The fix is to make the character survive long enough for it to feel consistent.

## Main Problems

### 1. Fire and cold resistance are undercapped

Current:

```text
Fire      43 / 75
Cold      38 / 75
Lightning 70 / 75
Chaos      0 / 75
```

This is the biggest immediate repair.

The character needs roughly:

```text
Fire:      +32
Cold:      +37
Lightning: +5
Chaos:     as much as practical, first target 20-30
```

Do not spend meaningful currency on damage before fire and cold are capped.

### 2. Boots are too light

Current boots:

- 20% movement speed
- cold resistance
- freeze duration reduction
- no life
- no second resistance

This is the cleanest first upgrade slot.

Target boots:

```text
25-30% movement speed
+maximum life
two useful resistances
optional chaos resistance / evasion / freeze utility
```

If one item fixes cold plus fire while adding life, the whole character immediately feels less fragile.

### 3. Ring 1 is mostly a leveling ring

The rare Topaz ring gives some flat attack damage, dexterity, small lightning resistance, and life on kill. It does not solve the current problem.

Replacement target:

```text
High fire or cold resistance
Second resistance or chaos resistance
maximum life
flat elemental attack damage if affordable
dexterity only if needed
```

The current Polcirkeln can stay because it supports the chill/shatter identity. The rare ring is the easier repair.

### 4. Amulet has Spirit but almost no survival

The amulet gives:

- `+39 Spirit`
- fire resistance
- evasion
- rarity

Spirit matters, so this is not a blind replacement. But the slot has no life, no cold resistance, no chaos resistance, and no damage mod that makes it sacred.

If reservation still works, a better amulet should look like:

```text
+Spirit
+maximum life
fire/cold/chaos resistance
projectile, attack, elemental, or cold damage if affordable
```

### 5. The jewel is off-plan

The current jewel:

- `5% increased Fire Damage`
- `16% increased Glory generation for Banner Skills`

For this character, that is close to a dead jewel.

Replace with a bow/cold/projectile jewel:

```text
Projectile damage
Attack damage
Cold damage
Elemental damage with attacks
Critical damage / ailment / freeze value
maximum life or resistance if available
```

This is a cheap, low-risk improvement.

## Repair Priority

### Phase 1: Make mapping stable

Goal:

```text
Life: 1700-1900+
Fire: 75
Cold: 75
Lightning: 75
Chaos: 20-30+
Movement speed: keep 25%+ if possible
```

Buy or craft in this order:

1. Boots with movement speed, life, and two resistances.
2. Rare ring replacing the Topaz ring with life and missing resistances.
3. Jewel replacing the fire/banner jewel with bow/cold/projectile value.
4. Amulet only if it preserves enough Spirit.

### Phase 2: Improve damage after the floor is fixed

Once the character is capped and no longer getting randomly killed:

1. Upgrade the bow for higher elemental DPS and projectile level.
2. Upgrade quiver for better flat damage, attack speed, crit, or projectile scaling.
3. Tune supports for the actual main skill that feels best in maps.
4. Consider whether Snipe is really winning boss fights; if not, move that socket pressure into a more reliable single-target setup.

## Slot-by-Slot Notes

### Keep for now

- Bow: good enough for level 68 repair stage.
- Body armour: strong life and useful resistances.
- Helmet: strong life.
- Belt: strong life and 3 charm slots.
- Polcirkeln: supports chill -> shatter identity.

### Replace soon

- Boots: needs life and more resistance.
- Rare ring: needs real resistance/life value.
- Jewel: current mods do not match the build.

### Replace carefully

- Amulet: Spirit is useful, but the rest of the slot is not strong enough long term.
- Gloves: good fire/lightning resistance and life-on-kill, but no life. Replace after boots/ring if survival still feels thin.

## Manual Trade Filter Recipes

### Boots

Required:

- `25%+ increased Movement Speed`
- `+# to maximum Life`
- two of fire / cold / lightning resistance

Strong adds:

- chaos resistance
- evasion
- freeze / chill utility

### Ring

Required:

- `+# to maximum Life`
- high fire or cold resistance
- second resistance or chaos resistance

Strong adds:

- flat cold/fire/lightning damage to attacks
- attack speed
- dexterity
- accuracy

### Amulet

Required:

- enough Spirit to keep reservations working
- maximum life or major resistance value

Strong adds:

- projectile damage
- elemental damage with attacks
- cold damage
- attributes

### Jewel

Required:

- projectile, attack, cold, or elemental attack damage

Strong adds:

- critical damage
- freeze / ailment value
- maximum life
- resistance

## Final Recommendation

Do the boring repair first:

```text
boots -> rare ring -> jewel
```

That should move the character from:

```text
undercapped early-map bow character
```

to:

```text
stable cold projectile Deadeye that can actually test its damage setup
```

Plain version: this is not a full rebuild. It is a resistance-and-floor repair. Cap fire/cold/lightning, get chaos off zero, replace the dead jewel, and only then pay for the next damage item.
