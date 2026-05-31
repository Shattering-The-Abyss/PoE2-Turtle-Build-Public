# Hollow Palm Monk Repair Demo

Date: 2026-05-31

Source:

- Public poe.ninja profile: <https://poe.ninja/poe2/profile/1793653506-1046/runesofaldur/character/%E6%A2%85%E5%A4%A7%E5%B8%9D>
- Character name: `Mei Emperor`
- Character level: `52`
- Class: `Monk`
- League: `Runes of Aldur`
- Snapshot checked from poe.ninja model data updated at `2026-05-31T03:30:45Z`

## Truth Boundary

This is a practical repair report based on the public poe.ninja character profile.

The analysis uses the public profile state: defensive panel, skill groups, equipped items, jewel, and keystone. It is not a full monster-damage simulation. The recommendations are triage: fix the survival-breaking problems first, then revisit damage.

## One-Line Diagnosis

The direction is real: `Hollow Palm Technique` plus `Storm Wave` gives the character a clear unarmed lightning Monk identity. The problem is not the damage idea. The problem is that the defensive floor is far too low for a character that wants to feel "unkillable."

## Current Character Read

```text
Level: 52
Class: Monk
Keystone: Hollow Palm Technique
Main skill: Storm Wave L12
Main support shell: Elemental Armament II / Shock / Branching Fissures I
```

Important current panel:

```text
Life: 882
Energy Shield: 42
Effective Health Pool: 905
Armour: 472
Evasion: 422
Fire Resistance: 14%
Cold Resistance: -9%
Lightning Resistance: -41%
Chaos Resistance: 15%
Lowest Maximum Hit Taken: 663
```

Main skill shell:

```text
Storm Wave L12
  Elemental Armament II
  Shock
  Branching Fissures I

Tempest Bell L6
  Magnified Area I
  Rage I

Frozen Locus L12
  Rapid Attacks I
  Magnified Area I

Ice Strike L7
  Rapid Attacks I
  Elemental Armament I

Glacial Cascade L4
  Elemental Armament I
  Rapid Attacks I
```

## What Is Working

The build has a coherent center.

`Hollow Palm Technique` requires both hand slots to be empty and lets unarmed attacks behave as quarterstaff attacks. That makes the empty weapon slots correct. The `Storm Wave` setup also makes sense for a lightning attack direction: `Elemental Armament II` fits, `Shock` fits the lightning plan, and `Branching Fissures I` helps clear.

There are also some usable pieces:

```text
Entropy March, Steeltoe Boots
  25% Movement Speed
  +94 Life
  Stun Threshold
  Reduced Shock duration

Plague Charm, Pearlescent Amulet
  +9% all elemental resistance implicit
  +46 Spirit
  +12 all attributes
  +15% Chaos Resistance

Havoc Keep, Visored Helm
  Accuracy
  Mana
  Critical Hit Chance
  +17% Cold Resistance
```

The issue is that these pieces do not add up to a stable defense package.

## Main Problems

### 1. Lightning Resistance Is Build-Breaking

Current lightning resistance:

```text
Lightning Resistance: -41%
```

This is the biggest hole in the character. The lowest maximum hit taken is also lightning:

```text
Lightning Maximum Hit Taken: 663
```

That means the character can die suddenly to lightning damage even if the main attack setup is correct.

Repair target:

```text
Lightning Resistance: move toward 75% immediately
Short-term target: at least positive, then 50%+
```

### 2. Cold And Fire Resistance Are Also Not Safe

Current elemental resistances:

```text
Fire Resistance: 14%
Cold Resistance: -9%
Lightning Resistance: -41%
```

This is not an "unkillable" baseline. It is a leveling character with a strong offensive idea and a weak defensive floor.

Repair targets:

```text
Fire Resistance: toward 75%
Cold Resistance: toward 75%
Lightning Resistance: highest urgency, toward 75%
```

### 3. Life Is Too Low For The Goal

Current life:

```text
Life: 882
```

At level 52, this is too thin for a character that wants to stand in danger and use melee-range attack skills.

Repair target:

```text
Life: 1200+ as the next practical checkpoint
Comfort target: 1500+ later
```

### 4. Ascendancy Is Missing

The profile reports:

```text
Ascendancy passive count: 0
```

If the character has not completed ascendancy trials yet, this is a major missing power source. The build should not spend too much effort fine-tuning small gear lines before claiming those points.

### 5. Some Item Slots Are Not Carrying Enough Survival

Helmet:

```text
No life
Only +17% Cold Resistance
Accuracy and mana are not solving the death problem
```

Ring:

```text
Gold Ring gives rarity and mana, but not enough life/resistance
```

Gloves:

```text
Useful offensive lines, but no life and only fire resistance
```

Jewel:

```text
4% Attack Speed is useful
Poison magnitude is mostly off-plan for a lightning Storm Wave setup
```

## Repair Plan

### Priority 1: Fix Lightning Resistance

Search for gear with:

```text
+Life
+Lightning Resistance
+Cold or Fire Resistance
```

Best early slots to fix this:

```text
Rings
Helmet
Belt
Gloves
Boots if a clear upgrade appears
```

### Priority 2: Replace Low-Survival Jewelry

The Gold Ring is not doing enough defensive work.

Look for:

```text
+Life
+Lightning Resistance
+Cold Resistance or Fire Resistance
Optional: attributes if needed
```

Do not overpay for rarity while the character is still dying.

### Priority 3: Replace Helmet

Search for:

```text
+Life
+Lightning Resistance
+Cold or Fire Resistance
Evasion / Energy Shield is a bonus for Hollow Palm scaling
```

For this character, a plain defensive helmet is better than a clever helmet that does not keep the character alive.

### Priority 4: Do Ascendancy

If ascendancy is still incomplete, finish it.

This is not a minor optimization. Zero ascendancy points means the character is missing a large part of class identity and power.

### Priority 5: Then Tune Damage

Only after the defensive floor is stable, revisit:

```text
Storm Wave support choices
Tempest Bell boss setup
Hollow Palm evasion / energy shield scaling
Attack speed
Lightning / elemental damage
Better jewel stats
```

## Final Verdict

This is not a failed build. It has a clear identity and the core skill setup is understandable.

The repair is:

```text
Keep Hollow Palm.
Keep Storm Wave as the main lane.
Fix lightning resistance immediately.
Fix cold/fire resistance next.
Raise life.
Complete ascendancy.
Then optimize damage.
```

Plain read: the engine is real, but the chassis is not ready for "unkillable" yet. Build the defensive floor first, then let the lightning Monk cook.
