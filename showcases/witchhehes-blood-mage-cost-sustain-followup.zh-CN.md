# WitchHehes 血法追踪分析：技能消耗怎么维持

来源：公开 poe.ninja 角色页面  
角色：`WitchHehes`，91 级 Blood Mage，Runes of Aldur  
相关报告：[WitchHehes 血法回血机制分析](witchhehes-blood-mage-recovery-analysis.zh-CN.md)

## 简短结论

这次补上的关键层不是“它怎么回血”。

更精确的问题是：

> 如果 Mana 通过 Mind Over Matter 变成防御血条，那它怎么避免技能把 Mana 花光？

答案是：

> 它把大量技能消耗从 Mana 挪到 Life，然后用 Life Remnants 把这个 Life 成本补回来。Mana 尽量保留给防御，再靠 Mana Remnants、击杀回蓝、蓝药补回来。

## 核心资源循环

```text
技能消耗 Life / 部分 Life
Life Remnants 补 Life
Mana 保留下来当 Mind Over Matter 防御池
Mana Remnants 在受伤或消耗后补 Mana
```

所以它不是简单的：

```text
Mana = Life
```

更准确是：

```text
Life 负责付技能费。
Mana 负责吃进来的伤害。
Remnants 同时补两个池子。
```

## 证据：Lifetap 到处都是

这些主动技能都带了 `Lifetap`：

- `Spark`
- `Lightning Bolt`
- `Orb of Storms`
- `Cast on Critical + Comet`
- `Frost Bomb`
- `Spellslinger + Living Bomb`
- `Elemental Weakness`

这是最大线索。这个 build 不希望普通施法把 Mana 池打空，因为 Mana 同时是防御池。

## 证据：武器把法术 Mana Cost 转成 Life Cost

它的 wand 有：

```text
16% of Spell Mana Cost Converted to Life Cost
```

这和 Lifetap 是同一个方向：

```text
降低 Mana 压力。
把施法成本转到 Life。
用 Remnants 把 Life 补回来。
```

这点尤其重要，因为它用了 `Eldritch Battery`，而 EB 会让 Mana Costs doubled。

## 为什么必须这样做

它用了：

```text
Mind Over Matter
Eldritch Battery
```

这两个 keystone 组合很强，但资源结构很别扭：

- `Mind Over Matter`: 所有伤害先从 Mana 扣，再扣 Life，但 Mana Recovery Rate 降低。
- `Eldritch Battery`: Energy Shield 转成最大 Mana，但 Mana Costs doubled。

如果它所有法术都用 Mana 支付，就会把自己用来防御的池子花掉。

所以它用 Life 去承担大部分施法成本。

## Life 成本怎么补

Life 侧靠：

```text
Life Remnants L20
Harmonic Remnants II
Remnant Potency III
```

观察到的数值：

```text
每个 Remnant 给 410 Life
Remnant Potency III 提高 40% effect
约等于每个 Life Remnant 给 574 Life
```

所以 `Life Remnants` 同时做两件事：

1. 补实际打到 Life 的伤害。
2. 补 Lifetap / 法术转 Life cost 花掉的 Life。

## Mana 防御池怎么补

Mana 侧靠：

```text
Mana Remnants L19
Harmonic Remnants II
Remnant Potency III
```

观察到的数值：

```text
每个 Remnant 给 311 Mana
Remnant Potency III 提高 40% effect
约等于每个 Mana Remnant 给 435 Mana
```

它还有一个 unique jewel 词缀：

```text
Recover 2% of maximum Mana on Kill
```

以 `3858 Mana` 计算，大约是：

```text
每击杀回 77 Mana
```

它也带了蓝药：

```text
29% of Recovery applied Instantly
48% increased Charges
```

所以刷图时 Mana 续航大概是：

- Mana Remnants
- 击杀回复 2% 最大 Mana
- 蓝药
- 通过 Lifetap 避免直接花太多 Mana

## 最终判断

这是一个双资源维持系统：

```text
Life 侧：
Lifetap / 转换成本 -> Life Remnants 补回来

Mana 侧：
Mind Over Matter 防御池 -> Mana Remnants / 击杀回蓝 / 蓝药补回来
```

如果只抄伤害链接，没抄资源循环，这个 build 很可能会翻车。贵的不只是 DPS，而是 Life 和 Mana 分工明确、各自能补。
