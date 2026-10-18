# WitchHehes 血法回血机制分析

来源：公开 poe.ninja 角色页面  
角色：`WitchHehes`，91 级 Blood Mage，Runes of Aldur  
URL: https://poe.ninja/poe2/builds/runesofaldur/character/Urbanspaghett-3756/WitchHehes?i=17&search=class%3DBlood%2BMage%26sort%3Ddps

## 简短结论

这个 build 不是主要靠传统吸血回血。

它的回复结构是一个分层的 Blood Mage / Archmage 生存系统：

1. `Life Remnants` 回血。
2. `Mana Remnants` 回蓝。
3. `Mind Over Matter` 让 Mana 先替 Life 吃伤害。
4. `Eldritch Battery` 把 Energy Shield 转成最大 Mana。
5. `Vitality II`、击杀回血、药水、护符提供小额兜底。

所以答案是：

> 它不是靠装备上一条明显的 leech 活着，而是靠 Remnant 循环回血/回蓝，并用大 Mana 池挡在 Life 前面。

## 观察到的防御面板

poe.ninja 当时数据：

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

重点是资源结构：血不高，蓝很高，ES 为 0。

这和它点的两个关键机制对上：

- `Mind Over Matter`: 所有伤害先从 Mana 扣，再扣 Life，但 Mana Recovery Rate 降低。
- `Eldritch Battery`: 把最大 Energy Shield 转成最大 Mana。

所以这里的 Mana 不是普通施法资源，而是第一层防御血条。

## 主回血：Life Remnants

技能连接：

```text
Life Remnants L20
Harmonic Remnants II
Remnant Potency III
```

`Life Remnants` 观察到的效果：

- Remnants 持续 8 秒。
- 击杀敌人有 25% 几率生成 Remnant。
- 命中目标时生成 Remnant，每 3 秒最多一次。
- 每个 Remnant 给 `410 Life`。

`Remnant Potency III` 提供：

- Supported Skill 生成的 Remnant 效果提高 40%。
- 收集后延迟 3 秒生效。

粗算一个 Life Remnant：

```text
410 * 1.4 = 574 Life
```

这才是它真正的 Life 回复引擎，只是不会像装备 leech 那样一眼看出来。

## 主防御回复：Mana Remnants

技能连接：

```text
Mana Remnants L19
Harmonic Remnants II
Remnant Potency III
```

`Mana Remnants` 观察到的效果：

- Remnants 持续 8 秒。
- 击杀带元素异常的敌人时有 25% 几率生成 Remnant。
- 暴击命中带元素异常的目标时生成 Remnant，每 2 秒最多一次。
- 每个 Remnant 给 `311 Mana`。

配合 `Remnant Potency III`，粗算：

```text
311 * 1.4 = 435 Mana
```

因为 `Mind Over Matter` 会让 Mana 先承伤，所以 Mana Remnants 实际上也是防御回复。

这就是这个 build 难看懂的地方：它把回复拆成两条线，一条补 Life，一条补 Mana 护城河。

## 次要回复来源

这些也存在，但不是核心：

### `Malice + Vitality II`

`Vitality II` 提供：

```text
Supported persistent buff active 时，每秒回复 2% maximum Life
```

以 `2682 Life` 计算：

```text
2682 * 0.02 = 53.6 Life/sec
```

poe.ninja 面板显示 `53/sec`，完全对上。

### 戒指击杀回血

一个戒指有：

```text
Gain 50 Life per enemy killed
```

对刷图有帮助，但不要当成 boss 战主要回复。

### 药水和护符

观察到的药水/护符回复：

- Life Flask: `920 Life over 3 seconds`
- Life Flask: `29% of recovery applied instantly`
- 腰带 implicit: `20% of flask recovery applied instantly`
- 护符：被晕时回复 `345 Life`

这些是紧急兜底或刷图辅助，不是主循环。

## 为什么容易看漏

如果只找这些关键词，很可能找不到答案：

- Life leech
- Damage leeched as Life
- 大量 regen
- instant Life on hit

真正的答案藏在技能和 keystone 组合里：

```text
Life Remnants + Mana Remnants + Mind Over Matter + Eldritch Battery
```

它同时维护两个池子：

- Life 靠 Life Remnants 补。
- Mana 靠 Mana Remnants 补，而 Mana 因为 MoM 先吃伤害，所以等于 Life 前面的第二血条。

## 抄作业注意点

如果要抄这个 build，不能只抄伤害技能。

回复包需要一起抄：

1. `Life Remnants`，并用 support 提高球的价值。
2. `Mana Remnants`，用来维持 Mana 防御池。
3. 足够暴击/元素异常，稳定触发 Mana Remnants。
4. 足够最大 Mana，让 `Mind Over Matter` 真有意义。
5. 操作上要能舒服吃球，因为 Remnants 需要捡。

如果这些缺了，角色可能看起来 DPS 很高，但实际会很脆。

