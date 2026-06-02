# MewOoooooO Invoker Comet Repair Report

Source: public poe.ninja character model for `MewOoooooO`, account `Chun_am#6252`, Runes of Aldur.

## Snapshot

- Level 89 `Invoker`
- Core engine: `Cast on Minion Death -> Comet`
- Scaling shell: `Archmage`, `Mind Over Matter`, `Eldritch Battery`, high maximum mana
- Comet shown by poe.ninja: about `26k` DPS
- Life: `1313`
- Mana: `3066`
- Spirit: `197`
- Resistances: Fire `75`, Cold `75`, Lightning `75`, Chaos `15`
- Lowest maximum hit taken: Physical `4714`
- Elemental maximum hit taken: about `16307`
- Chaos maximum hit taken: `5372`

## Short Verdict

This is not a directionless character. The idea is clear:

```text
Invoker shell
-> mana stack / Archmage
-> MoM + Eldritch Battery
-> Cast on Minion Death
-> Comet as payoff
-> Wolf Pack / minion death as trigger fuel
```

The problem is not the concept. The problem is that the engine is more advanced than the chassis. The build is asking mana and trigger mechanics to cover for a very thin life pool, low physical hit floor, and only modest chaos resistance.

The first repair is not "buy more DPS". The first repair is making the character stop collapsing when mana gets pressured.

## What Is Working

### Weapon

The wand is real for this setup:

- `+4 to Level of all Cold Spell Skills`
- spell damage
- extra cold damage
- crafted spell critical chance
- elemental gain rune

This is not the emergency slot.

### Amulet

The amulet is very on-lane:

- `+41 Spirit`
- `+13 Spirit` implicit
- `+1 to Level of all Spell Skills`
- high mana
- lightning / chaos resistance

It supports reservation, mana scaling, and spell level at the same time. Do not replace it casually.

### Jewels

The Sapphire jewels are coherent:

- spell damage
- triggered spell damage
- critical damage
- cast speed or mana-on-kill utility

That is the correct kind of jewel direction for a triggered Comet build.

### Elemental Resistances

Fire, cold, and lightning are capped. Lightning even has meaningful overcap. Elemental resistance is not the current crisis.

## Main Problems

### 1. Life is too low for level 89

`1313` life is the biggest warning.

Because this is a `Mind Over Matter` character, life is not the whole defensive pool. But life still matters when mana gets drained, when chaos damage lands, or when physical spikes punch through.

Repair target:

```text
Keep the mana shell,
but move gear from "mana only" toward "mana + life" or "mana + life + resistance".
```

### 2. Physical maximum hit is the weakest defensive number

Physical maximum hit taken is only about `4714`.

The character has only moderate armour, almost no evasion, modest block, and no obvious large physical conversion layer. That means elemental hits can look fine while physical rares, bosses, or bad map mods suddenly kill the character.

Repair target:

```text
Raise the physical hit floor before buying luxury damage.
```

### 3. Chaos resistance is functional, not comfortable

Chaos resistance is `15%`. That is not a disaster, but with only `1313` life it is still a real failure mode.

Repair target:

```text
Push chaos resistance toward 35-50% without breaking mana, Spirit, or spell levels.
```

### 4. Doedre's Tenure may be damage bait

`Doedre's Tenure` gives huge spell damage, but it does not solve life, mana, or defensive stability. It also has reduced cast speed.

It can still be acceptable because Comet is being triggered, not normally self-cast. But if boss deaths are the problem, rare gloves with life, mana, resistance, and useful caster stats should be tested even if tooltip DPS drops.

## Repair Priority

### 1. Belt or shield first

The current belt has lightning resistance and armour, but no life and only small mana. The shield has all-res and intelligence, but also no life.

Search for:

```text
Belt or Shield
- maximum life
- maximum mana or mana recovery
- chaos resistance or all elemental resistance

Good extras:
- armour
- block chance / defensive shield value
- intelligence
- strength if attribute pressure exists
```

Why first:

This directly repairs the likely death pattern without touching the trigger engine.

### 2. Upgrade body armour only if Spirit is preserved

The current body armour carries `+43 Spirit`, multiple resistances, and bonded life/mana. It is doing a job.

A real upgrade needs:

```text
+Spirit
+maximum life
+maximum mana or strong Energy Shield converted through Eldritch Battery
+resistance or chaos resistance
```

If a replacement loses too much Spirit, reservations can break.

### 3. Test rare gloves against Doedre's Tenure

Rare glove target:

```text
- life
- mana
- resistance / chaos resistance
- cast speed, spell damage, or triggered spell damage if affordable
```

If the character dies less even with lower paper DPS, that is a successful repair.

### 4. Damage upgrades come after the floor is stable

After survival stabilizes, continue scaling:

- better spell level weapon
- better spell level / mana / Spirit amulet
- stronger triggered spell jewels
- Comet gem level / quality
- better `Cast on Minion Death` support setup

## Market Filter Recipes

Use these as manual trade filter recipes.

### Belt

```text
Category: Belt
Required:
- +# to maximum Life
- +# to maximum Mana
- +#% to Chaos Resistance OR +#% to all Elemental Resistances

Optional:
- Armour
- Strength / Intelligence
- Flask mana recovery
- Charm slots
```

### Shield

```text
Category: Shield
Required:
- +# to maximum Life
- +# to maximum Mana OR high Energy Shield
- +#% to all Elemental Resistances OR Chaos Resistance

Optional:
- Block chance
- Armour / Energy Shield
- Intelligence
```

### Gloves

```text
Category: Gloves
Required:
- +# to maximum Life
- +# to maximum Mana
- at least one useful resistance

Optional:
- Cast Speed
- Spell Damage
- Triggered Spell Damage
- Intelligence
```

### Jewels

```text
Category: Sapphire Jewel or relevant spell jewel
Required:
- Triggered Spells deal increased Spell Damage OR Spell Damage
- Critical Damage Bonus

Optional:
- Cast Speed
- maximum Mana
- Mana on Kill
- defensive suffix
```

## Skill Engine Check

The current engine is understandable:

- `Cast on Minion Death L16 Q20`
- `Comet L19 Q20`
- `Spell Cascade`
- `Boundless Energy II`
- `Efficiency II`
- `Wolf Pack L17 Q20`
- `Minion Instability`
- `Minion Mastery`
- `Amanamu's Tithe`
- `Archmage L19 Q23`
- `Grim Feast`

The real question is not only "is Comet damage high enough?"

The real question is:

```text
Can the build produce enough minion deaths,
generate enough trigger energy,
pay the mana costs,
and survive until the next Comet cycle?
```

## Plain Recommendation

Keep the identity:

```text
Invoker
Archmage
MoM + EB
Cast on Minion Death
Comet
Wolf Pack trigger fuel
```

Repair the floor:

1. Buy or craft a belt/shield with real life + mana + chaos or defensive value.
2. Test rare gloves if boss deaths matter more than tooltip damage.
3. Do not casually lose Spirit on body armour or amulet.
4. Continue damage scaling only after physical/chaos/life are less fragile.

Human version: the engine is clever, but the chassis is too thin. Fix the chassis first, then tune the engine.
