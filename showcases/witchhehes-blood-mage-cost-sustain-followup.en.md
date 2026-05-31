# WitchHehes Blood Mage Follow-Up: How Skill Costs Are Sustained

Source: public poe.ninja character page  
Character: `WitchHehes`, Level 91 Blood Mage, Runes of Aldur  
Related report: [WitchHehes Blood Mage Recovery Analysis](witchhehes-blood-mage-recovery-analysis.en.md)

## Short Verdict

The missing layer is not only "how does this build recover Life?"

The sharper question is:

> If Mana is the defensive life buffer through Mind Over Matter, how does the build avoid spending all of that Mana on skills?

The answer:

> It moves a large part of skill cost away from Mana and into Life, then uses Life Remnants to refill that Life cost. Mana is preserved for defense and refilled separately by Mana Remnants, kill Mana, and flask support.

## The Core Resource Loop

```text
Skills spend Life / partial Life
Life Remnants refill Life
Mana is preserved as the Mind Over Matter buffer
Mana Remnants refill Mana after damage or spending
```

So the build is not simply:

```text
Mana = Life
```

It is closer to:

```text
Life pays for casting.
Mana pays for incoming damage.
Remnants refill both pools.
```

## Evidence: Lifetap Is Everywhere

The following active setups include `Lifetap`:

- `Spark`
- `Lightning Bolt`
- `Orb of Storms`
- `Cast on Critical + Comet`
- `Frost Bomb`
- `Spellslinger + Living Bomb`
- `Elemental Weakness`

That is the major clue. The build does not want normal casting to drain the Mana pool because Mana is also its defensive buffer.

## Evidence: Wand Converts Spell Mana Cost To Life Cost

The wand has:

```text
16% of Spell Mana Cost Converted to Life Cost
```

This points in the same direction as Lifetap:

```text
Reduce pressure on Mana.
Move casting cost into Life.
Use Remnants to refill Life.
```

This matters even more because the build uses `Eldritch Battery`, which doubles Mana costs.

## Why This Is Necessary

The build uses:

```text
Mind Over Matter
Eldritch Battery
```

Those keystones create a powerful but awkward resource structure:

- `Mind Over Matter`: all damage is taken from Mana before Life, but Mana Recovery Rate is reduced.
- `Eldritch Battery`: Energy Shield becomes maximum Mana, but Mana Costs are doubled.

If the character paid all spell costs with Mana, it would spend the same pool it needs for defense.

The build solves that by letting Life pay for much of the casting load.

## Life Cost Sustain

The Life side is supported by:

```text
Life Remnants L20
Harmonic Remnants II
Remnant Potency III
```

Observed value:

```text
410 Life per Remnant
40% increased effect from Remnant Potency III
Approx. 574 Life per Life Remnant
```

This means `Life Remnants` is doing two jobs:

1. recovering from damage that reaches Life
2. paying back Life spent through Lifetap / converted spell cost

## Mana Buffer Sustain

The Mana side is supported by:

```text
Mana Remnants L19
Harmonic Remnants II
Remnant Potency III
```

Observed value:

```text
311 Mana per Remnant
40% increased effect from Remnant Potency III
Approx. 435 Mana per Mana Remnant
```

The build also has a unique jewel roll:

```text
Recover 2% of maximum Mana on Kill
```

At `3858 Mana`, that is roughly:

```text
77 Mana per kill
```

It also uses a Mana Flask with:

```text
29% of Recovery applied Instantly
48% increased Charges
```

So in mapping, Mana sustain is likely a combination of:

- Mana Remnants
- 2% maximum Mana recovered on kill
- Mana flask
- not spending too much Mana directly because Lifetap shifts costs away

## Final Read

This is a two-pool sustain engine:

```text
Life side:
Lifetap / converted costs -> Life Remnants refill

Mana side:
Mind Over Matter damage buffer -> Mana Remnants / kill Mana / flask refill
```

If someone copies only the damage links and misses the resource loop, the build can fail badly. The expensive part is not just DPS; it is keeping Life and Mana assigned to different jobs.
