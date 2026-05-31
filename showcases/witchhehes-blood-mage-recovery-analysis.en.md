# WitchHehes Blood Mage Recovery Analysis

Source: public poe.ninja character page  
Character: `WitchHehes`, Level 91 Blood Mage, Runes of Aldur  
URL: https://poe.ninja/poe2/builds/runesofaldur/character/Urbanspaghett-3756/WitchHehes?i=17&search=class%3DBlood%2BMage%26sort%3Ddps

## Short Verdict

This build is not mainly recovering through classic leech.

The recovery package is a layered Blood Mage / Archmage setup:

1. `Life Remnants` restores Life.
2. `Mana Remnants` restores Mana.
3. `Mind Over Matter` makes Mana function as the first life buffer.
4. `Eldritch Battery` converts Energy Shield into more maximum Mana.
5. Small passive recovery comes from `Vitality II`, kill recovery, flask, and charm effects.

So the answer is:

> The build survives by cycling Remnants and protecting Life behind a large Mana pool, not by relying on visible leech.

## Observed Defensive State

From poe.ninja at time of review:

- Life: `2682`
- Mana: `3858`
- Energy Shield: `0`
- Life Regeneration: `53/sec`
- Effective Health Pool: `15542`
- Physical Max Hit: `7447`
- Fire Max Hit: `26550`
- Cold Max Hit: `17288`
- Lightning Max Hit: `26550`
- Chaos Max Hit: `20650`

The unusual part is the resource layout: low visible Life, high Mana, zero ES.

That makes sense because the build uses:

- `Mind Over Matter`: all damage is taken from Mana before Life, with less Mana Recovery Rate.
- `Eldritch Battery`: converts maximum Energy Shield into maximum Mana.

This means Mana is not just a casting resource. It is the first defensive buffer.

## Main Life Recovery: Life Remnants

The build uses:

```text
Life Remnants L20
Harmonic Remnants II
Remnant Potency III
```

Observed `Life Remnants` stats:

- Remnants last 8 seconds.
- 25% chance to spawn a Remnant on killing an enemy.
- Spawn a Remnant on hitting a target, no more than once every 3 seconds.
- Each Remnant grants `410 Life`.

`Remnant Potency III` adds:

- Remnants from supported skills have 40% increased effect.
- Effects occur 3 seconds after being collected.

Approximate effective value:

```text
410 * 1.4 = 574 Life per Life Remnant
```

This is the real Life recovery engine. It just does not look like normal leech on the gear sheet.

## Main Defensive Recovery: Mana Remnants

The build also uses:

```text
Mana Remnants L19
Harmonic Remnants II
Remnant Potency III
```

Observed `Mana Remnants` stats:

- Remnants last 8 seconds.
- 25% chance to spawn a Remnant on killing an enemy affected by an elemental ailment.
- Spawn a Remnant on critically hitting a target affected by an elemental ailment, no more than once every 2 seconds.
- Each Remnant grants `311 Mana`.

With `Remnant Potency III`, approximate effective value:

```text
311 * 1.4 = 435 Mana per Mana Remnant
```

Because `Mind Over Matter` routes damage to Mana before Life, Mana Remnants are indirectly defensive recovery.

That is why this build can look confusing: the recovery is split between Life pickup and Mana buffer refill.

## Minor Recovery Sources

These are real, but secondary:

### `Malice + Vitality II`

`Vitality II` gives:

```text
Regenerate 2% of maximum Life per second while a supported persistent buff is active
```

At `2682 Life`, that is about:

```text
2682 * 0.02 = 53.6 Life/sec
```

poe.ninja shows `53/sec`, so this matches the sheet.

### Ring Kill Recovery

One ring has:

```text
Gain 50 Life per enemy killed
```

This helps mapping but should not be treated as boss sustain.

### Flask And Charm

Observed flask/charm recovery:

- Life Flask: `920 Life over 3 seconds`
- Life Flask: `29% of recovery applied instantly`
- Belt implicit: `20% of flask recovery applied instantly`
- Charm: recover `345 Life` when stunned

These are emergency or mapping support layers, not the main engine.

## Why It Is Easy To Miss

If you only scan for these terms, you will not find the answer:

- Life leech
- Damage leeched as Life
- massive regen
- instant Life on hit

The build's recovery is hidden in its skill setup and keystone interaction:

```text
Life Remnants + Mana Remnants + Mind Over Matter + Eldritch Battery
```

The player is maintaining two pools:

- Life through Life Remnants.
- Mana through Mana Remnants, which protects Life because of Mind Over Matter.

## Practical Takeaway

If copying this build, do not copy only the damage setup.

The recovery package requires:

1. `Life Remnants` supported for stronger pickup value.
2. `Mana Remnants` supported for Mana buffer sustain.
3. Enough crit / ailment application to generate Mana Remnants reliably.
4. Enough maximum Mana to make `Mind Over Matter` meaningful.
5. Comfortable movement and pickup behavior, because Remnants need to be collected.

If those pieces are missing, the build may show high DPS but feel fragile.

