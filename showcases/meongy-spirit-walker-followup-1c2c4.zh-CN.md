# Spirit Walker 伙伴召唤后续报告：Meongy 1c2c4

日期：2026-05-31

来源：

- 更新后的 poe.ninja PoB：<https://poe.ninja/poe2/pob/1c2c4>
- 原始修车报告：[Meongy Spirit Walker 伙伴召唤修车报告](meongy-spirit-walker-companion-repair.zh-CN.md)

## 真实性边界

这是针对更新后角色状态的后续报告。

它不替代原始报告。原始报告定位的是紧急修车优先级；这份报告检查她改了什么，以及下一层修车应该往哪里走。

## 一句话诊断

这次更新是一次很成功的修车。

角色修掉了最危险的问题：电抗不再是负数，鞋子修好了，手套修好了，Spirit 不再完全卡死，而且装备上已经有更多真正支持 companion 路线的东西。

下一个问题已经不是“这车坏了”。现在的问题是收束优化：继续抬高防御地板，换掉低价值戒指和盾牌，同时在强化 companion 体系时保留 Spirit 弹性。

## 快照对比

原始报告：

```text
等级：65
生命：1499
能量护盾：26
Spirit：1
未保留 Spirit：0
火抗：43%
冰抗：9%
电抗：-9%
混沌抗：7%
```

更新后 1c2c4：

```text
等级：71
生命：1696
能量护盾：185
Mana：681
Spirit：100
未保留 Spirit：19
护甲：546
闪避：1590
闪避率：15%
格挡：0%
火抗：56%
冰抗：44%
电抗：74%
混沌抗：28%
```

改善点：

```text
生命：+197
能量护盾：+159
电抗：-9% -> 74%
冰抗：9% -> 44%
火抗：43% -> 56%
混沌抗：7% -> 28%
Spirit 弹性：0 未保留 -> 19 未保留
```

这是实质修车，不是表面变化。

## 当前技能壳

主要 companion 组合：

```text
Companion: Diretusk Boar L14
  Feeding Frenzy I
  Hulking Minions I
  Rapid Attacks I

Companion: Diretusk Boar L14
  Bleed IV
```

其他工具：

```text
Wolf Pack L14
Tame Beast L13
Discipline L14

Twister L11
  Elemental Armament II
  Frost Nexus
  Retreat I

Whirling Slash L11
  Rapid Attacks I
  Cadence
  Rage I

Barrage L10
Raise Shield
Spear Throw
```

判断：

```text
这现在更明显是一只 Spirit Walker companion 角色。
它不再只是借用 companion 工具。
武器和技能组已经开始直接支持这条路线。
```

## 她修对了什么

### 1. 鞋子修好了

新鞋：

```text
Vengeance Stride, Bastion Sabatons
20% increased Movement Speed
+85 maximum Life
+39 maximum Mana
+27% Cold Resistance
+27% Lightning Resistance
Rune/enchant 额外给 Lightning Resistance、Life、Mana
```

结论：

```text
非常好的修车。
这正是原始报告想要的鞋子方向。
除非出现明显升级，否则保留。
```

### 2. 手套修好了

新手套：

```text
Mind Fingers, Commander Gauntlets
+64 maximum Life
+53 maximum Mana
+32% Fire Resistance
+24% Cold Resistance
+26% Lightning Resistance
Rune/enchant 额外给 Cold Resistance、Life、Mana
```

结论：

```text
非常好的修车。
这个槽位已经从弱填充变成真正的防御支点。
保留。
```

### 3. Spirit 和 companion 武器包改善很大

重要武器：

```text
Victory Gnarl, Stoic Sceptre
Spirit: 100
Grants Level 14 Discipline
Allies in your Presence deal 68% increased Damage
Allies in your Presence deal 1 to 35 added Attack Lightning Damage
+2 to Level of all Minion Skills
Minions have 44% increased maximum Life
Rune/enchant: Companions deal 30% increased Damage
```

结论：

```text
这是货真价实的 Spirit Walker / companion 路线装备。
它解决了之前 Spirit 卡死的问题，并且给了直接的 minion / ally scaling。
除非出现非常贵且明显更强的版本，否则保留。
```

### 4. companion 伤害武器也是真的

另一把长矛：

```text
Dire Edge, Branched Spear
Companions deal 50% increased Damage
48% increased Damage while your Companion is in your Presence
Physical damage and life/mana on kill
```

结论：

```text
这是路线相关装备，不是随机伤害。
现在装备上已经有真正的 companion scaling。
```

## 剩余问题

### 1. 冰抗和火抗变好了，但还没完成

当前抗性：

```text
Fire: 56%
Cold: 44%
Lightning: 74%
Chaos: 28%
```

电抗在这个阶段基本修好了。

冰抗仍然是最弱的元素抗。火抗能玩，但也应该继续往上补。

下一目标：

```text
Cold: 往 75% 推
Fire: 往 75% 推
Lightning: 保持接近上限
Chaos: 保持正数，后面再慢慢补
```

### 2. 戒指现在是最明显升级区

当前戒指：

```text
Dragon Finger, Ruby Ring
+25% Fire Resistance implicit
+4% all Elemental Resistances
+26% Fire Resistance
+14% Chaos Resistance
No Life

Tempest Whorl, Prismatic Ring
+9% all Elemental Resistances implicit
+21% Lightning Resistance
+14% Chaos Resistance
+28 Intelligence
No Life
```

结论：

```text
戒指帮忙解决了一部分抗性压力，但两个都没有生命。
现在鞋子和手套已经修好，戒指应该成为下一轮购买或制作目标。
```

理想戒指形状：

```text
+Life
+Cold Resistance
+Fire Resistance or all Elemental Resistances
Attributes or Mana if needed
Chaos Resistance as bonus
```

现在不要为戒指上的伤害词缀多花钱。

### 3. 盾牌偏弱

当前盾牌：

```text
Carrion Bastion, Crescent Targe
+13 maximum Life
+8% Fire Resistance
+7% Chaos Resistance
Raise Shield
```

结论：

```text
这现在是可见装备里最弱的槽位之一。
它还能用，只是因为其他装备已经把角色救起来了。
戒指之后升级；如果市场上有便宜且明显更好的盾牌，也可以提前换。
```

好盾牌目标：

```text
+60 maximum Life or better
Two useful resistances, preferably Cold + Fire
Block or defensive base value
Spirit only if available cheaply
```

### 4. Spirit 变好了，但仍然偏紧

当前：

```text
Spirit: 100
Unreserved Spirit: 19
```

这比之前好很多，但还不算宽裕。

后续任何 companion 组合、光环、保留或辅助调整，都应该先检查 Spirit 再决定。

## 更新后的修车优先级

### 优先级 1：带生命和冰抗的戒指

最实际的下一步，是找一枚能补 Life 和 Cold Resistance，同时不破坏 Lightning 的戒指。

搜索目标：

```text
Ring
Required Level <= 71
+50 maximum Life or better
+25% Cold Resistance or better
One of:
  +Fire Resistance
  +All Elemental Resistances
  +Chaos Resistance
  +Attributes / Mana
```

### 优先级 2：第二枚戒指或盾牌，看价格

如果戒指便宜，先修两枚戒指。

如果盾牌明显便宜，第二枚戒指之前先换盾也可以。

盾牌搜索目标：

```text
Shield
Required Level <= 71
+60 maximum Life or better
+25% Cold Resistance or better
+25% Fire Resistance or all Elemental Resistances
Block or good defensive base as bonus
```

### 优先级 3：保留 minion 等级装备

不要随便换掉：

```text
+2 minion helmet
+2 minion amulet
Spirit/minion sceptre
companion damage spear
fixed boots
fixed gloves
```

这些是 build identity 装备，或者高价值修车成果。

### 优先级 4：最后才追伤害

伤害不是现在的紧急问题。

角色已经有：

```text
+2 minion helmet
+2 minion amulet
+2 minion sceptre
companion damage weapon/rune support
minion/companion jewels
```

下一步升级应该先让角色更稳、更顺。

## 更新后的个性化 Filter 说明

当前个性化 filter 仍然有用：

- [Meongy Spirit Walker Level 65 Loot Filter](../loot-filters/meongy-spirit-walker-level-65.filter)

但这次更新后，最重要的高亮槽位变成：

```text
Rings
Shields
Jewels
Charms
Currency
```

鞋子和手套可以继续高亮，但已经不再紧急，因为当前鞋子和手套都很好。

## 最终结论

这是一次成功修车。

人话版：

```text
保留新鞋子。
保留新手套。
保留 +2 minion 头和项链。
保留 Spirit/minion sceptre。
保留 companion damage 武器。
下一步先修戒指，再修盾牌。
冰抗和生命是下一阶段最实际目标。
防御地板更干净前，不要重金追伤害。
```

原始诊断被这次更新验证了：方向是对的，地板是不够的。装备地板一抬起来，整个角色马上变得清晰很多。
