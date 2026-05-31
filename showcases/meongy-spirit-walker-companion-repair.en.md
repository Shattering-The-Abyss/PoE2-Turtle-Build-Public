# Spirit Walker Companion Repair: Meongy

Date: 2026-05-31

Source:

- Public poe.ninja PoB link: <https://poe.ninja/poe2/pob/1c236>
- Character level: `65`
- Class: `Huntress`
- Ascendancy: `Spirit Walker`

## Truth Boundary

This is a practical repair report based on a public poe.ninja PoB export.

The analysis uses the current character state: defensive panel, skills, items, and the visible Spirit Walker companion direction. It is not a final meta build guide and not a full damage simulation.

## One-Line Diagnosis

This character is already on the intended lane: `Huntress -> Spirit Walker -> companion / turtle-style survival`. The build direction is not wrong. The main issue is that the companion core is ahead of the defensive and resource floor.

## Current Character Read

```text
Level: 65
Class: Huntress
Ascendancy: Spirit Walker
Life: 1499
Energy Shield: 26
Mana: 620
Spirit: 1
Unreserved Spirit: 0
Effective Health Pool: 2499
Armour: 637
Evasion: 1438
Block: 26%
Fire Resistance: 43%
Cold Resistance: 9%
Lightning Resistance: -9%
Chaos Resistance: 7%
```

Main skill shell:

```text
Companion: Diretusk Boar L12
  Feeding Frenzy I
  Hulking Minions I
  Rapid Attacks I

Twister L11
  Elemental Armament II
  Frost Nexus
  Retreat I

Whirling Slash L11
  Rapid Attacks I
  Cadence
  Rage I

Tame Beast L12
Barrage L10
Raise Shield
Spear Throw
```

## What Is Working

This build already has real companion-route assets.

Important keepers:

```text
Amulet:
  +99 maximum Life
  +2 to Level of all Minion Skills

Helmet:
  +99 maximum Life
  +2 to Level of all Minion Skills
  Deflection scaling from Evasion

Belt:
  +85 maximum Life
  +22% Cold Resistance
  +29% Lightning Resistance

Body Armour:
  +127 maximum Life
  +20% Fire Resistance
  Armour/Evasion base

Shield:
  +29 maximum Life
  +15% Fire Resistance
  +13% Cold Resistance
  +10% Lightning Resistance
```

The `+2 minion` amulet and helmet are especially important. They are route assets, not random leveling trash.

## Main Problems

### 1. Spirit Is Too Tight

Current panel:

```text
Spirit: 1
Unreserved Spirit: 0
```

For a Spirit Walker companion build, this is the main resource warning. The build is functioning, but it has almost no Spirit flexibility. Any future reservation, aura, companion package, or support change can hit a wall.

This does not mean the current setup is wrong. It means future upgrades should watch Spirit carefully.

### 2. Cold And Lightning Resistances Are Not Ready

Current resistances:

```text
Fire: 43%
Cold: 9%
Lightning: -9%
Chaos: 7%
```

Fire is acceptable for the moment. Cold and lightning are not. Lightning being negative is the biggest danger.

Short-term target:

```text
Lightning: positive immediately, then toward 75%
Cold: 50%+ next, then toward 75%
Fire: keep improving toward 75%
Chaos: keep non-negative
```

### 3. Boots Are The Clearest Upgrade Slot

Current boots:

```text
Viper Hoof, Covered Sabatons
+78 Mana
+22% Cold Resistance
No Life
No Movement Speed
```

At level 65, no movement speed and no life is too expensive. This is the first slot to replace.

### 4. Gloves Are Also Weak

Current gloves:

```text
+29 maximum Life
+87 maximum Mana
+22 Intelligence
+178 Accuracy
```

This is usable as a temporary item, but accuracy is not the main stat for the companion plan. The slot should do more defensive work.

### 5. Rings Are Transitional

One ring carries a lot of fire resistance but no life. The other has all resistance and intelligence, but also no life. These are usable, but they should eventually become life + lightning/cold resistance slots.

## Repair Plan

## Personalized Loot Filter

Download:

- [Meongy Spirit Walker Level 65 Loot Filter](../loot-filters/meongy-spirit-walker-level-65.filter)
- Raw download link after merge: <https://raw.githubusercontent.com/Shattering-The-Abyss/PoE2-Turtle-Build-Public/main/loot-filters/meongy-spirit-walker-level-65.filter>

Filter purpose:

```text
Highlight rare boots, gloves, rings, and shields for the current repair plan.
Keep currency, uncut gems, jewels, and charms visible.
Do not hide everything else yet; this is a safe personalized repair filter, not a strict endgame loot filter.
```

Important limitation:

```text
The in-game filter cannot inspect unidentified affixes like +60 life or +25 lightning resistance.
It highlights the item classes worth identifying based on the repair priorities below.
```

### Priority 1: Replace Boots

Look for:

```text
20%+ Movement Speed
+60 maximum Life or better
+Lightning Resistance
+Cold or Fire Resistance
```

This is the highest-value immediate repair.

### Priority 2: Replace Gloves

Look for:

```text
+60 maximum Life or better
Two useful resistances
Attributes or Mana as a bonus
Defensive base is a bonus
```

Do not pay for attack accuracy unless the player personally needs it for the current hybrid play feel.

### Priority 3: Clean Up Rings

Look for:

```text
+Life
+Lightning Resistance
+Cold Resistance or Fire Resistance
Attributes / Mana if needed
```

The goal is not fancy damage. The goal is making the companion route safer.

### Priority 4: Upgrade Shield Later

The current shield is fine as a low-level resistance shield, but it can eventually be upgraded.

Look later for:

```text
+Life
+Block
+Two resistances
Armour/Evasion or Armour/ES base
Spirit if available cheaply
```

## Do Not Rush To Replace

Keep these for now:

```text
+2 minion amulet
+2 minion helmet
Life body armour
Life + cold/lightning belt
```

These are not perfect, but they support the actual direction.

## Trade Search Filters

Use these as minimum filters, not luxury filters. Start cheap, then widen price only if no reasonable results appear.

### Boots

Search category:

```text
Armour -> Boots
Required Level <= 65
```

Minimum filters:

```text
+60 to maximum Life
20% increased Movement Speed
+25% to Lightning Resistance
One of:
  +25% to Cold Resistance
  +25% to Fire Resistance
```

Good extras:

```text
Evasion or Armour/Evasion base
Mana
Attributes
Rarity only if free
```

### Gloves

Search category:

```text
Armour -> Gloves
Required Level <= 65
```

Minimum filters:

```text
+60 to maximum Life
Two elemental resistances
```

Preferred resistance pairing:

```text
Lightning + Cold
```

Good extras:

```text
Mana
Dexterity / Intelligence
Armour/Evasion or Evasion/ES base
Minion-related stats if cheap
```

### Ring

Search category:

```text
Accessory -> Ring
Required Level <= 65
```

Minimum filters:

```text
+40 to maximum Life
+25% to Lightning Resistance
One of:
  +25% to Cold Resistance
  +25% to Fire Resistance
```

Good extras:

```text
All Elemental Resistances
Mana
Attributes
Minion damage only if cheap
```

### Shield

This is lower priority than boots/gloves/rings.

Search category:

```text
Off Hand -> Shield
Required Level <= 65
```

Minimum filters:

```text
+60 to maximum Life
+20% to Lightning Resistance
+20% to Cold or Fire Resistance
```

Good extras:

```text
Block
Armour/Evasion base
Spirit if cheap
```

### Buying Order

```text
1. Boots
2. Gloves
3. Ring
4. Shield only if cheap and clearly better
```

Do not spend the first currency on damage. The current route already has minion-skill support. The first shopping goal is to stabilize movement speed, life, lightning resistance, and cold resistance.

## Final Verdict

This is a real Spirit Walker companion character. The direction should be preserved.

Plain read:

```text
Keep the +2 minion helmet and amulet.
Keep the companion lane.
Replace boots first.
Replace gloves second.
Use rings to fix lightning and cold resistance.
Watch Spirit carefully before adding more reservations.
```

The build is not failing because the plan is wrong. It just needs the defensive floor to catch up with the companion idea.
