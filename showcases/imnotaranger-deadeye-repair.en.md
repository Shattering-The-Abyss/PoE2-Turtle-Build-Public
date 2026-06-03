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

## Updated Boss-Damage Verdict

The player report is: boss fights take about two minutes, the character has to play like Contra, and damage feels absent.

That read is credible. The first version of this report correctly identified the defensive floor problem, but the boss complaint changes the priority: this is not only a resistance repair. The character also needs a damage-engine rebuild.

The current boss-damage warning signs are concrete:

- Main skill gems are only `L14 Q0`.
- `Ice Shot` shows only `9375` DPS.
- `Snipe`, which should be the aimed burst button, shows only `2799` DPS.
- `Tornado Shot` shows only `4559` DPS and is more coverage than boss payoff here.
- The bow is `1.20` attacks per second and has no attack speed, no critical strike scaling, and only modest flat elemental damage.
- The rare ring, amulet, jewel, and quiver are not carrying enough boss damage.
- `Polcirkeln` is useful for chill/shatter mapping identity, but it is not a boss-killing engine by itself.

So the real diagnosis is:

```text
Mapping idea exists.
Boss engine does not.
Defensive floor is also too low, so every long boss fight becomes a bullet-hell fight.
```

If the fight lasts two minutes, every defensive weakness gets amplified. The character is not merely dying because it is fragile; it is fragile for too long.

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

The first repair is not a luxury bow, but the first real rebuild must include damage. Capping resistances alone will make the two-minute boss fight safer, not shorter.

## What Is Working

### Bow

The bow is good enough for the current stage:

- `+1 to Level of all Projectile Skills`
- added physical and fire damage
- increased elemental damage with attacks
- cold rune damage
- mana leech from physical damage
- extra dexterity

This is not a useless bow, but it is probably no longer enough if the complaint is boss time.

The problem is not one missing mod. It is the whole boss profile:

```text
1.20 attacks per second
modest flat elemental damage
no attack speed
no critical strike scaling
no high end-game elemental DPS
```

`+1 projectile skills` is nice, but it cannot carry boss damage alone.

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

### 0. There is no real boss-kill setup yet

The current skill sheet is split across several attacks:

```text
Ice Shot L14 Q0      -> clear
Tornado Shot L14 Q0  -> coverage
Snipe L14 Q0         -> intended burst, but low displayed DPS
Barrage L14 Q0       -> utility/cooldown package, not a visible damage core
```

For mapping, this can feel okay. For bosses, the build needs one clear answer:

```text
What button actually kills the boss?
```

Right now the answer is not strong enough. `Snipe` is not carrying, `Tornado Shot` is not built as the boss payoff, and `Ice Shot` is still in a clear-oriented setup with `Fork`.

Boss repair target:

```text
Pick one single-target plan,
then make bow, quiver, supports, jewels, and jewelry serve that plan.
```

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

### Phase 0: Stop the boss from being a two-minute fight

This is the new priority after the player feedback.

Do these before buying luxury defensive pieces:

1. Level the main skill gems. `L14 Q0` is too low for a character trying to push bosses.
2. Replace the current jewel. Fire damage plus banner glory is basically not part of this build.
3. Decide the boss button: either make `Snipe` a real single-target setup, or move toward an `Ice Shot`/`Barrage` boss package.
4. Prepare a boss gem swap if keeping `Fork` for mapping. `Fork` is a clear support; it should not be treated as the boss answer.

### Phase 1: Repair damage and floor together

Goal:

```text
Life: 1700-1900+
Fire: 75
Cold: 75
Lightning: 75
Chaos: 20-30+
Movement speed: keep 25%+ if possible
Main damage skill: higher gem level, better supports, real boss plan
```

Buy or craft in this order:

1. Jewel replacing the fire/banner jewel with bow/cold/projectile value.
2. Rare ring replacing the Topaz ring with life, missing resistances, and flat elemental attack damage if possible.
3. Boots with movement speed, life, and two resistances.
4. Quiver upgrade if affordable: flat elemental damage, projectile damage, attack speed, critical value, or accuracy.
5. Bow upgrade when budget allows: higher elemental DPS, attack speed, and projectile skill level.

### Phase 2: Real boss rebuild

Once the character is capped enough to play:

1. Upgrade the bow for higher elemental DPS, attack speed, and projectile level.
2. Upgrade quiver for flat elemental damage, projectile damage, attack speed, crit, or accuracy.
3. Move jewelry from "random useful stats" toward "life/resist plus attack damage".
4. Tune supports around the actual boss skill, not around clear.
5. If `Snipe` still does not beat just attacking, drop it as the boss plan.

## Slot-by-Slot Notes

### Keep for now

- Bow: acceptable for early mapping, but not a long-term boss weapon.
- Body armour: strong life and useful resistances.
- Helmet: strong life.
- Belt: strong life and 3 charm slots.
- Polcirkeln: supports chill -> shatter identity.

### Replace soon

- Boots: needs life and more resistance.
- Rare ring: needs real resistance/life value and ideally attack damage.
- Jewel: current mods do not match the build.
- Quiver: current flat damage is useful, but it lacks the stronger boss scaling expected from this slot.

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

### Bow

Required:

- much higher elemental DPS than the current bow
- attack speed, or a clearly stronger total damage profile
- projectile skill level if available

Strong adds:

- flat cold damage
- flat lightning or fire damage
- critical strike chance / critical damage direction
- accuracy or dexterity if needed

### Quiver

Required:

- flat elemental damage to attacks
- projectile damage or attack speed

Strong adds:

- critical damage / critical chance direction
- accuracy
- dexterity
- resistance if it prevents another slot from becoming defensive-only

## Final Recommendation

Do the correct rebuild first:

```text
jewel -> rare ring -> boots -> quiver -> bow
```

That should move the character from:

```text
undercapped early-map bow character with no boss engine
```

to:

```text
stable cold projectile Deadeye with a real boss button
```

Plain version: the first report was too gentle for the boss complaint. If bosses take two minutes, this is a damage-engine repair, not only a resistance repair. Cap the character enough to stop panic-playing, but spend the upgrade path on the parts that actually shorten the fight: gem levels, jewel, rare ring, quiver, bow, and boss supports.
