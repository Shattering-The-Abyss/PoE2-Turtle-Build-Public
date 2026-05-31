# Blood Mage Repair Demo

Date: 2026-05-30

Source:

- Imported from a player-provided Path of Building export.
- Character level: `53`
- Class: `Witch`
- Ascendancy: `Blood Mage`

## Truth Boundary

This is a practical build-repair report based on a PoB export.

The analysis uses the exported character state: defensive panel, skill groups, equipped items, jewels, and weapon-set configuration.

It is not a full monster-damage simulation. The recommendations are triage: fix the most obvious build-breaking problems first, then revisit damage.

## One-Line Diagnosis

The character has a real idea: Blood Mage, minion death trigger, Comet, Wolf Pack, and spell / crit scaling. The problem is not imagination. The problem is that the defensive floor and resource setup are not stable enough for the idea yet.

## Current Character Read

```text
Level: 53
Class: Witch
Ascendancy: Blood Mage
Main idea: Cast on Minion Death -> Comet
Support idea: Wolf Pack / Minion Instability / Elemental Weakness / Life Remnants
```

Important current panel:

```text
Life: 870
Effective Health Pool: 1063
Armour: 170
Evasion: 156
Fire Resistance: 45%
Cold Resistance: 55%
Lightning Resistance: -18%
Chaos Resistance: 0%
Spirit: 50
Unreserved Spirit: -65
```

Main skill shell:

```text
Cast on Minion Death L10
  Comet L13
  Spell Cascade
  Boundless Energy II
  Energy Retention

Resonating Shield L5
  Minion Pact II
  Steadfast II

Elemental Weakness L12
  Heightened Curse
  Prolonged Duration II

Wolf Pack L13
  Minion Instability

Grim Feast L10
Life Remnants L13
Sigil of Power L8
```

## What Is Working

The build has a recognizable plan.

`Cast on Minion Death -> Comet` is a real engine idea. `Wolf Pack` and `Minion Instability` point toward using minion bodies as a trigger / explosion layer. `Elemental Weakness` supports the spell damage plan, and `Life Remnants` / `Grim Feast` fit the Blood Mage survival theme.

There are some useful item pieces:

```text
Rattling Sceptre
  +125 Spirit
  +1 to Level of all Minion Skills
  Grants Skeletal Warrior

Sire of Shards
  104% increased Spell Damage
  16% increased Cast Speed
  Spells fire 4 additional Projectiles

Shield
  +56 Life
  Fire Resistance
  Cold Resistance
  Stun Threshold
```

The problem is that these pieces are pulling the character in different directions.

## Main Problems

### 1. Lightning Resistance Is Build-Breaking

Current lightning resistance is:

```text
Lightning Resistance: -18%
```

At level 53, that is the first repair target. This is not a small optimization issue. It is the kind of hole that causes sudden deaths even if the damage engine works.

Repair target:

```text
Lightning Resistance: at least 50%+
Ideal: 75%
```

### 2. Life Is Too Low For Blood Mage

Current life:

```text
Life: 870
```

This is low for a Blood Mage using a costly trigger / spell shell. The export also shows meaningful life cost pressure:

```text
Life Cost: 73
Life per Second Cost: 41.9
```

That means the character is paying life while also taking incoming damage. With low life and negative lightning resistance, the build can fail before its engine gets to perform.

Repair target:

```text
Life: 1100-1300+ as the next practical checkpoint
```

### 3. Spirit / Weapon-Set Logic Is Not Stable

The export shows:

```text
Spirit: 50
Unreserved Spirit: -65
```

This suggests the current selected setup does not support the intended reservations / minions, or that the active weapon set in PoB is not aligned with how the character is actually played.

There are two competing weapon identities:

```text
Sceptre + Shield:
  more Spirit
  +minion skill level
  Skeletal Warrior
  safer defensive posture

Sire of Shards:
  stronger spell projectile fantasy
  extra projectiles
  less minion / Spirit stability
```

The character should not try to be both at the same time until the resource math works.

### 4. Boots And Helmet Are Outdated

Boots:

```text
10% Movement Speed
+20 Mana
+10% Cold Resistance
+13% Lightning Resistance
```

These are too weak for level 53. They do not solve the lightning problem, do not add life, and only give low movement speed.

Helmet:

```text
+41 Accuracy
Item Rarity
Critical Hit Chance
+11% Fire Resistance
```

Accuracy is mostly wasted for this spell / minion / trigger shell. This slot should be doing life and resist work.

### 5. Jewels Are Directional But Not Emergency Fixes

Current jewels contain spell crit, crit damage, ignite magnitude, and one plant damage line.

These are not the main problem. They may support a spell crit plan, but they should not be tuned before lightning resistance, life, and Spirit are fixed.

## Repair Plan

### Priority 1: Replace Boots

Search for:

```text
20%+ Movement Speed
+60 Life or better
+25% Lightning Resistance or better
Any second resistance
```

This is likely the highest-value single item fix.

### Priority 2: Replace Helmet

Search for:

```text
+Life
+Lightning Resistance
+Fire or Cold Resistance
Energy Shield or Armour/Energy Shield base is fine
```

Do not pay for accuracy on this build.

### Priority 3: Decide The Main Weapon Identity

If the build is primarily minion-trigger Blood Mage:

```text
Prefer sceptre + shield for now.
Stabilize Spirit.
Keep minion levels and defensive shield value.
```

If the build is primarily Sire of Shards Comet:

```text
Accept that Spirit/minion setup must be rebuilt around the staff.
Do not assume the sceptre minion package is still available.
```

Current recommendation:

```text
Use sceptre + shield until the defensive and Spirit floor are fixed.
Treat Sire of Shards as a promising damage toy, not the foundation yet.
```

### Priority 4: Revisit Damage After The Floor Is Stable

Only after the character has:

```text
Lightning Resistance near cap
Fire/Cold moving toward cap
1100-1300+ Life
Non-negative Spirit budget
```

Then tune:

```text
Comet support choices
Spell crit jewels
Minion death trigger uptime
Sire of Shards swap plan
```

## Final Verdict

This is not a failed build. It is an interesting build that reached the point where the idea is ahead of the chassis.

The correct repair is:

```text
Fix lightning resistance.
Raise life.
Stabilize Spirit.
Choose one main weapon identity.
Then optimize Comet / crit / minion death scaling.
```

Plain read: the fireworks idea is real, but the character needs tires and brakes before more explosives.
