# Martial Artist To Comet Minion Conversion Review

Date: 2026-05-31

Source:

- Public poe.ninja PoB link: <https://poe.ninja/poe2/pob/1c1ef>
- Player-provided video reference screenshots for a `Cast on Minion Death -> Comet` route.
- Passive tree respec reference: <https://www.poe2wiki.net/wiki/Passive_skill_tree>

## Truth Boundary

This is a conversion-readiness report, not a finished build guide.

The current character is a level 81 Monk / Martial Artist. The target idea is a minion-death-triggered Comet setup, apparently based on a Blood Mage / Witch-style route shown in the reference screenshots. The recommendation below separates hard current-character facts from conversion assumptions.

## One-Line Diagnosis

This is not a small respec. The current character is an attack / quarterstaff / crit Martial Artist. The target setup is a minion / trigger / spell / Spirit / curse shell. Converting is possible, but it is closer to rebuilding the vehicle than tuning it.

## Current Character Read

```text
Level: 81
Class: Monk
Ascendancy: Martial Artist
Current main skill: Killing Palm L12
Current weapon: rare Sinister Quarterstaff
Allocated passive nodes: 114
```

Important current panel:

```text
Life: 1538
Energy Shield: 60
Effective Health Pool: 1647
Armour: 27
Evasion: 201
Fire Resistance: 27%
Cold Resistance: 4%
Lightning Resistance: -18%
Chaos Resistance: 8%
Spirit: 1
Unreserved Spirit: -89
```

Current skill shell:

```text
Killing Palm L12
  Charge Profusion I
  Thrill of the Kill
  Blazing Critical

Pounce L3
  Rapid Attacks II
  Compressed Duration I

Lingering Illusion L13
  Prolonged Duration I

Charge Regulation L14
Wind Dancer L14
```

## Target Build Read From Screenshots

The referenced route appears to center around:

```text
Summon Wolf / wolf package
Cast on Minion Death
Comet
Grim Feast
Resonating Shield
Elemental Weakness
Frost Bomb
Archmage, if using the mana-scaling variant
```

The screenshot also notes:

```text
Wolf setup wants about 120 Spirit.
Summon Pact should be adjusted around player/minion life.
If wolf life is low, use level 1 pact.
Wolf should only be placed in weapon set 1, otherwise a resurrection bug may fail.
```

## Which Monk Ascendancy Fits?

If the player insists on staying Monk, the practical answer is:

```text
Invoker > Acolyte of Chayula > Martial Artist
```

### Invoker

Invoker is the least awkward Monk option because it has more natural overlap with elemental and spell-oriented scaling. If this conversion must remain a Monk, Invoker is the first place to test.

### Acolyte of Chayula

Acolyte of Chayula is not the first recommendation for this plan. It points more toward chaos / darkness / resource mechanics. That may be interesting, but it is not the cleanest match for a Comet minion-death shell.

### Martial Artist

Martial Artist is the wrong shell for this conversion. The current character is already built around attack identity: Killing Palm, quarterstaff, crit, and melee routing. Keeping Martial Artist while trying to become a minion-trigger spell build wastes too much of the ascendancy identity.

## Best Class For The Target Idea

If the question is "what is best for this exact target build?", the answer is probably not Monk.

The video route looks much closer to:

```text
Witch / Blood Mage
```

Blood Mage naturally connects to life, spell cost, spell scaling, Life Remnants / Grim Feast-style survival, and the broader minion-trigger identity. A Monk conversion can be done, but it is a retrofit.

## Gold Cost Estimate

The current tree has:

```text
114 allocated passive nodes
```

At level 81, the wiki respec table lists about:

```text
3089 gold per passive point
```

Estimated cost:

```text
30-point adjustment: about 92,670 gold
60-point rebuild: about 185,340 gold
90-point rebuild: about 278,010 gold
114-point full reset: about 352,146 gold
```

This conversion is not a 30-point adjustment. A realistic budget is:

```text
Minimum: 300k gold
Comfortable: 400k+ gold
Testing / mistakes included: 500k+ gold
```

If ascendancy-class swapping is unavailable or expensive in the current patch state, the cost is even harder to justify.

## What Can Stay

### Usable For Now

Helmet:

```text
Hate Star, Tribal Mask
  +166 maximum Life
  +79 maximum Mana
  +33% Cold Resistance
```

This is not perfect, but it has real life and mana.

Ruby Ring:

```text
Behemoth Spiral
  +54 maximum Life
  +11% all Elemental Resistances
  +28% Fire Resistance
  +22% Lightning Resistance
```

This ring is usable as a transition item.

Amethyst Ring:

```text
Golem Grasp
  +49 maximum Life
  +12 all Attributes
  +8% Chaos Resistance implicit
```

This has useful life and attributes, but the attack damage and mana leech lines become less valuable after converting away from attacks.

## What Must Change

### Weapon

The current `Sinister Quarterstaff` is an attack weapon. It does not belong in the target shell.

The conversion wants something closer to:

```text
High Spirit source
Minion skill levels
Spell skill levels or spell damage
Mana / attributes if using Archmage
```

### Amulet

The current amulet has:

```text
+1 to Level of all Melee Skills
```

That is off-plan for Comet/minion/spell conversion. Replace with:

```text
+Spirit
+spell/minion-relevant levels or damage
+life
+resistances
+attributes if needed
```

### Empty Gear Slots

The current PoB has empty:

```text
Body Armour
Gloves
Boots
```

This is a major conversion blocker. Those slots must carry life, resistances, Spirit/resource support, and defense before the new build will feel stable.

### Resistances

Current resistances are not ready:

```text
Fire: 27%
Cold: 4%
Lightning: -18%
Chaos: 8%
```

Before converting, target:

```text
Elemental resistances near 75%
Lightning fixed first
Chaos at least non-negative
```

## Preparation Checklist

Before spending the gold:

```text
1. Confirm whether Monk ascendancy can be swapped cleanly.
2. Prepare at least 300k-400k gold.
3. Acquire the required skill gems.
4. Acquire the required support gems.
5. Build a 120 Spirit plan.
6. Fill body armour, gloves, and boots.
7. Fix lightning resistance.
8. Simulate the new tree before committing.
9. Decide whether this is really worth doing instead of leveling a Witch / Blood Mage.
```

## Practical Recommendation

If the player wants to experiment and keep the Monk identity:

```text
Swap toward Invoker if possible.
Do not keep Martial Artist as the final shell.
Prepare 400k+ gold.
Buy the Spirit and resistance gear first.
Only respec after the skill package is ready.
```

If the player wants the cleanest version of the video build:

```text
Level a Witch / Blood Mage instead.
```

## Final Verdict

This conversion is possible, but it is expensive and structurally awkward.

Plain read: the current Martial Artist is a melee attack car. The target Comet minion build is a spell-trigger engine. You can weld the engine into the car, but if the goal is to follow the video cleanly, a Blood Mage chassis is probably the better base.
