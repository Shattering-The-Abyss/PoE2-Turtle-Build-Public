# Random Level 70 Tactician Repair Demo

Date: 2026-05-30

Source character:

- Character: `SexySchoolGirlxz`
- Account: `Vladilena_-6547`
- League: `Runes of Aldur`
- Class: `Tactician`
- Level: `70`
- Public page: <https://poe.ninja/poe2/builds/runesofaldur/character/Vladilena_-6547/SexySchoolGirlxz>

## Truth Boundary

This is a public build-repair demo using poe.ninja character data.

The analysis uses the public character payload: defensive panel, items, skill links, jewels, passive count, and visible build structure.

It is not a full monster-damage simulation. Without current monster tables, zone modifiers, player execution, and death logs, the repair plan should be read as practical triage rather than exact survival math.

## One-Line Diagnosis

This character is not broken. It is a working crossbow elemental Tactician with a clear damage plan, but the defensive shell is under-budgeted for level 70.

## Current Read

Core identity:

```text
Crossbow Tactician
Stormblast Bolts / Galvanic Shards
Herald of Thunder support shell
Elemental attack scaling
```

Important defensive panel:

```text
Life: 1321
Energy Shield: 64
Effective Health Pool: 2130
Movement Speed: 111%
Armour: 43
Evasion: 304
Evade Chance: 3%
Fire Resistance: 36%
Cold Resistance: 75%
Lightning Resistance: 54%
Chaos Resistance: 0%
Lowest Maximum Hit Taken: 1353
```

Main skill links:

```text
Stormblast Bolts L14
  Elemental Armament II
  Ice Bite II
  Rapid Attacks I
  Close Combat I

Galvanic Shards L15
  Elemental Armament I
  Double Barrel III
  Fork
  Mobility

Mirage Archer L12
  Prolonged Duration I
  Explosive Shot
  Cooldown Recovery II

Herald of Thunder L13
  Elemental Armament I
  Elemental Focus
  Deadly Herald
```

## What Is Working

The attack identity is coherent. The character is clearly trying to use crossbow skills, elemental scaling, Herald damage, and projectile / attack tempo.

The weapon is serviceable:

```text
Spirit Core Cannonade Crossbow
130% increased Physical Damage
Adds Physical Damage
Crafted Cold Damage
Fire and Lightning rune damage
Grenade Skills fire an additional Projectile
```

The boots are strong for progression:

```text
20% Movement Speed
+103 Life
+39 Mana
+27% Fire Resistance
+26% Lightning Resistance
Lightning rune resistance
Life regeneration
```

The body armour is doing important build work:

```text
Enfolding Dawn
+100 Spirit
+15% all Elemental Resistances
Fire resistance rune
```

## Main Problems

### 1. Fire and Lightning Resistance Are Not Capped

Cold resistance is fine at `75%`, but fire is only `36%` and lightning is only `54%`.

At level 70, this is the biggest repair priority. The character can look functional during normal clear and then get deleted by the wrong elemental hit.

Repair target:

```text
Fire Resistance: 75%
Lightning Resistance: 75%
Cold Resistance: keep capped
Chaos Resistance: improve later, but do not chase it before fire/lightning are fixed
```

### 2. Physical Defense Is Very Thin

The character has:

```text
Armour: 43
Evasion: 304
Evade Chance: 3%
Physical Maximum Hit Taken: 1389
```

That means the character is mostly relying on killing speed, positioning, and recovery. This is playable, but it is not sturdy.

Repair target:

```text
Add more life where possible.
Prefer armour/evasion bases that do not destroy the resistance plan.
Do not trade capped elemental resistance away for small damage gains.
```

### 3. Jewels Have Mismatched Mods

The two rare Emerald jewels include useful Herald damage, but also bow-specific and poison stats:

```text
Luminous Bloom
  13% increased Accuracy Rating with Bows
  10% chance to Poison on Hit
  Herald Skills deal 25% increased Damage

Armageddon Hope
  7% increased Damage with Bows
  9% chance to Poison on Hit
  Herald Skills deal 24% increased Damage
  Debuffs expire 8% faster
```

For a crossbow character, the bow lines are mostly wasted. The Herald lines are useful, but these jewels are not clean fits.

Better jewel targets:

```text
Projectile damage
Attack damage
Elemental damage with attacks
Lightning damage
Attack speed
Accuracy if actually needed
Life or resistance if available
```

## Repair Plan

Priority 1:

```text
Cap Fire Resistance and Lightning Resistance.
```

Do this through rings, amulet, helmet, belt, or rune choices before touching the main damage setup.

Priority 2:

```text
Replace mismatched jewels.
```

Keep Herald damage if possible, but stop paying jewel budget for bow-only lines on a crossbow character.

Priority 3:

```text
Add more life and real mitigation.
```

The character's movement speed and damage shell can carry progression, but the defensive numbers are low for harder content.

Priority 4:

```text
Only upgrade the weapon after the resistance floor is stable.
```

The current crossbow is good enough to keep playing. A damage upgrade is nice, but it should not come before the defensive fix.

## Final Verdict

This is a functional build with a clear plan. The fix is not to rebuild the character from zero.

The correct repair is:

```text
Keep the crossbow elemental shell.
Cap fire and lightning resistance.
Replace bow/poison jewel waste.
Add more life or mitigation.
Then revisit weapon damage.
```

The practical read: the engine runs, but the chassis is too light.
