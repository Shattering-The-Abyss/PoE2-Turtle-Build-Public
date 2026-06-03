# imnotaranger Deadeye 修车报告

来源：poe.ninja 公开角色模型，角色 `imnotaranger`，账号 `nega_tive#4060`，Runes of Aldur。

本次快照：

- poe.ninja profile: <https://poe.ninja/poe2/profile/nega_tive-4060/runesofaldur/character/imnotaranger>
- poe.ninja 最后检查时间：`2026-06-03T02:44:03Z`
- Level 68 `Deadeye`
- 主要技能壳：`Ice Shot`、`Tornado Shot`、`Snipe`、`Freezing Mark`
- 面板 DPS：`Ice Shot 9375`、`Tornado Shot 4559`、`Snipe 2799`
- Life: `1536`
- Energy Shield: `272`
- Mana: `530`
- Spirit: `139`
- Movement speed: `128%`
- 抗性：Fire `43`、Cold `38`、Lightning `70`、Chaos `0`
- 最低 maximum hit taken：Chaos `1672`
- Physical maximum hit taken：`1900`

这份报告只基于 poe.ninja 公开快照；没有包含地图录像、死亡日志、仓库预算或实际手感。

## Boss 伤害深挖结论

玩家反馈是：打一个 Boss 大概两分钟，过程像魂斗罗，角色没伤害。

这个判断可信。第一版报告抓到了防御底盘问题，但这个 Boss 主诉会改变优先级：这不只是补抗性的小修，这套角色还需要伤害引擎大修。

当前 Boss 伤害警讯很具体：

- 主技能都是 `L14 Q0`。
- `Ice Shot` 只有 `9375` DPS。
- 本来应该负责瞄准爆发的 `Snipe` 只有 `2799` DPS。
- `Tornado Shot` 只有 `4559` DPS，而且当前更像覆盖技能，不是 Boss payoff。
- 弓只有 `1.20` attacks per second，没有 attack speed，没有 crit scaling，flat elemental damage 也不够高。
- rare ring、amulet、jewel、quiver 没有一起承担 Boss 伤害。
- `Polcirkeln` 对 chill / shatter 清图身份有用，但它本身不是 Boss 击杀引擎。

真实诊断是：

```text
清图思路存在。
Boss 引擎不存在。
防御底盘也太低，所以每个长 Boss 都会变成弹幕求生。
```

如果 Boss 打两分钟，所有防御缺点都会被放大。角色不是单纯因为脆才死，而是因为要脆很久。

## 简短结论

这车不是技能方向错了。冷系弓投射物的想法是成立的：

```text
+1 projectile bow
Ice Shot 清图
Tornado Shot 覆盖
Snipe 尝试单体爆发
Freezing Mark / Herald of Ice / Combat Frenzy 工具层
Polcirkeln 负责 chill -> shatter 转换
```

真正的问题更简单：

```text
输出已经想开始刷图，
但防御底盘还停在剧情 / 早期地图水平。
```

Level 68 时，火抗和冰抗没满，混沌抗是 0，chaos 和 physical 最大承伤都低于 `2000`。所以实战会很随机：有些怪能炸得很爽，但遇到强 rare、地面效果、混沌伤害或物理尖刺时，会在弓技能开始发挥之前直接倒。

第一步不是无脑买高级弓，但真正的大修必须包含伤害。只补抗性会让两分钟 Boss 更安全，不会让它变短。

## 现在能用的部分

### Bow

这把弓在当前阶段够用：

- `+1 to Level of all Projectile Skills`
- 附加 physical / fire damage
- increased elemental damage with attacks
- cold rune damage
- physical damage mana leech
- dexterity

这把弓不是废品，但如果主诉是 Boss 时间，它大概率已经不够了。

问题不是少一条词缀，而是整个 Boss 画像太弱：

```text
1.20 attacks per second
flat elemental damage 偏低
没有 attack speed
没有 critical strike scaling
没有高端 elemental DPS
```

`+1 projectile skills` 很好，但不能单独承担 Boss 伤害。

### Body Armour

胸甲是目前比较好的装备：

- `+198 maximum Life`
- fire / cold resistance
- energy shield
- life regeneration

除非新胸甲同时提升 life 和抗性，否则先保留。

### Helmet / Belt

头和腰带都有很高 life：

- Helmet: `+165 maximum Life`
- Belt: `+158 maximum Life`，3 charm slots

它们在撑底盘。可以以后升级，但不是第一轮乱换的对象。

### 冷系弓身份

技能包足够清楚：

- `Ice Shot` 主清图
- `Tornado Shot` 覆盖
- `Snipe` 单点爆发尝试
- `Freezing Mark`
- `Herald of Ice`
- `Combat Frenzy`
- `Wind Dancer`

这个身份可以继续。修车目标是让角色活到这套东西稳定运转。

## 主要问题

### 0. 现在没有真正的 Boss 击杀方案

当前技能表分散在几个攻击上：

```text
Ice Shot L14 Q0      -> 清图
Tornado Shot L14 Q0  -> 覆盖
Snipe L14 Q0         -> 预期爆发，但面板很低
Barrage L14 Q0       -> 工具 / 冷却包，不是可见伤害核心
```

清图时这可能还行。打 Boss 时，build 需要一个明确答案：

```text
到底哪个按钮负责杀 Boss？
```

现在答案不够强。`Snipe` 没扛起来，`Tornado Shot` 没被做成 Boss payoff，`Ice Shot` 还带着偏清图的 `Fork`。

Boss 修车目标：

```text
先选定一个单体方案，
然后让 bow / quiver / supports / jewels / jewelry 都服务这个方案。
```

### 1. 火抗和冰抗没满

当前：

```text
Fire      43 / 75
Cold      38 / 75
Lightning 70 / 75
Chaos      0 / 75
```

这是最优先修的问题。

大概需要补：

```text
Fire:      +32
Cold:      +37
Lightning: +5
Chaos:     能补多少补多少，第一目标 20-30
```

火冰没满之前，不建议投入明显成本去买纯伤害。

### 2. Boots 太薄

当前鞋子：

- 20% movement speed
- cold resistance
- reduced freeze duration
- 没 life
- 没第二条抗性

这是最干净的第一升级槽。

目标鞋子：

```text
25-30% movement speed
+maximum life
两条有效抗性
可选 chaos resistance / evasion / freeze utility
```

如果一双鞋能同时补 cold、fire、life，整车会立刻稳很多。

### 3. Rare ring 更像练级戒指

当前 Topaz rare ring 给了一些 flat attack damage、dexterity、小 lightning resistance 和 life on kill。它没有解决当前核心问题。

替换目标：

```text
高 fire 或 cold resistance
第二抗性或 chaos resistance
maximum life
如果买得起，再带 flat elemental attack damage
dexterity 只在缺属性时需要
```

Polcirkeln 可以先保留，因为它服务 chill / shatter 身份。rare ring 更适合先修。

### 4. Amulet 有 Spirit，但生存价值不足

项链给：

- `+39 Spirit`
- fire resistance
- evasion
- rarity

Spirit 有用，所以不能盲目换。但这个槽位没有 life、没有 cold resistance、没有 chaos resistance，也没有强到必须保留的伤害词。

如果 reservation 不会坏，后续项链应该找：

```text
+Spirit
+maximum life
fire/cold/chaos resistance
projectile / attack / elemental / cold damage
```

### 5. Jewel 基本不在计划内

当前 jewel：

- `5% increased Fire Damage`
- `16% increased Glory generation for Banner Skills`

对这套角色来说，这接近一颗死珠宝。

换成弓 / 冷 / 投射物珠宝：

```text
Projectile damage
Attack damage
Cold damage
Elemental damage with attacks
Critical damage / ailment / freeze value
maximum life or resistance if available
```

这是便宜、低风险、很干净的升级。

## 修车顺序

### Phase 0：先让 Boss 不再打两分钟

这是根据玩家反馈更新后的新优先级。

在买昂贵纯防御装之前，先做这些：

1. 主技能宝石升级。`L14 Q0` 对想打 Boss 的角色来说太低。
2. 换掉当前 jewel。Fire damage + banner glory 基本不属于这套 build。
3. 明确 Boss 按钮：要么把 `Snipe` 做成真正单体，要么转向 `Ice Shot` / `Barrage` 的 Boss 包。
4. 如果保留 `Fork` 清图，就准备 Boss gem swap。`Fork` 是清图 support，不应该当 Boss 答案。

### Phase 1：伤害和底盘一起修

目标：

```text
Life: 1700-1900+
Fire: 75
Cold: 75
Lightning: 75
Chaos: 20-30+
Movement speed: 尽量保住 25%+
Main damage skill: 更高 gem level，更合理 support，明确 Boss 方案
```

购买 / 制作顺序：

1. Jewel：把 fire/banner 珠宝换成 bow/cold/projectile 方向。
2. Rare ring：替换 Topaz ring，补 life、缺失抗性，最好再带 flat elemental attack damage。
3. Boots：movement speed + life + two resistances。
4. Quiver：预算允许时找 flat elemental damage、projectile damage、attack speed、crit value 或 accuracy。
5. Bow：预算允许时换更高 elemental DPS、attack speed、projectile skill level 的弓。

### Phase 2：真正重做 Boss 伤害

等角色有基本抗性、能站住以后：

1. 升级更高 elemental DPS、attack speed、projectile level 的弓。
2. 升级 quiver，找 flat elemental damage、projectile damage、attack speed、crit 或 accuracy。
3. Jewelry 从“随机有用词缀”改成“life/resist + attack damage”。
4. Support 围绕真正 Boss 技能调整，不围绕清图。
5. 如果 `Snipe` 仍然打不过普通攻击循环，就不要继续把它当 Boss 方案。

## 槽位建议

### 先保留

- Bow：早期刷图能用，但不是长期 Boss 武器。
- Body armour：life 和抗性不错。
- Helmet：life 很好。
- Belt：life 很好，3 charm slots。
- Polcirkeln：服务 chill -> shatter 身份。

### 尽快替换

- Boots：需要 life 和更多抗性。
- Rare ring：需要真正的抗性 / life 价值，最好还带 attack damage。
- Jewel：当前词缀和 build 不匹配。
- Quiver：当前 flat damage 有用，但缺少这个槽位该提供的 Boss scaling。

### 谨慎替换

- Amulet：Spirit 有用，但长期看其余词缀不够强。
- Gloves：fire/lightning 抗性和 life-on-kill 有用，但没有 life。鞋子和戒指修完后，如果还脆，再看手套。

## 手动市场 Filter

### Boots

必须：

- `25%+ increased Movement Speed`
- `+# to maximum Life`
- fire / cold / lightning resistance 中的两条

加分：

- chaos resistance
- evasion
- freeze / chill utility

### Ring

必须：

- `+# to maximum Life`
- 高 fire 或 cold resistance
- 第二抗性或 chaos resistance

加分：

- flat cold/fire/lightning damage to attacks
- attack speed
- dexterity
- accuracy

### Amulet

必须：

- 足够 Spirit，保证 reservation 不坏
- maximum life 或明显抗性价值

加分：

- projectile damage
- elemental damage with attacks
- cold damage
- attributes

### Jewel

必须：

- projectile / attack / cold / elemental attack damage

加分：

- critical damage
- freeze / ailment value
- maximum life
- resistance

### Bow

必须：

- 比当前弓高很多的 elemental DPS
- attack speed，或者总伤害画像明显更强
- 如果有预算，带 projectile skill level

加分：

- flat cold damage
- flat lightning / fire damage
- critical strike chance / critical damage 方向
- accuracy / dexterity

### Quiver

必须：

- flat elemental damage to attacks
- projectile damage 或 attack speed

加分：

- critical damage / critical chance 方向
- accuracy
- dexterity
- resistance，如果它能避免其他槽位变成纯防御装

## 最终建议

先做正确的大修：

```text
jewel -> rare ring -> boots -> quiver -> bow
```

目标是从：

```text
抗性没满、没有 Boss 引擎的早期地图弓角色
```

变成：

```text
有明确 Boss 按钮的冷系投射物 Deadeye
```

人话版：第一版报告对 Boss 主诉太温和了。如果 Boss 要打两分钟，这就是伤害引擎修复，不只是抗性修复。抗性要补到不慌，但升级路线必须花在能缩短战斗的部位：gem level、jewel、rare ring、quiver、bow、Boss supports。
