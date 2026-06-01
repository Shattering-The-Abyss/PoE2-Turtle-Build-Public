# 梅大帝 Martial Artist 修车报告

日期：2026-05-31

来源：

- 公开 poe.ninja 角色页：<https://poe.ninja/poe2/profile/1793653506-1046/runesofaldur/character/%E6%A2%85%E5%A4%A7%E5%B8%9D>
- 角色名：`梅大帝`
- 角色等级：`63`
- 职业：`Martial Artist`
- 联赛：`Runes of Aldur`

## 真实性边界

这是基于公开 poe.ninja 角色数据做的实战修车报告。

本报告不是完整怪物伤害模拟，也不是精算版 build planner。这里做的是修车 triage：先看角色为什么容易死、哪些装备槽最拖后腿、哪些问题应该先修，避免一上来就追输出导致越改越歪。

## 一句话诊断

这台车不是发动机坏了，是底盘漏风。

`Hollow Form / Storm Wave / elemental Martial Artist` 的方向能看懂，主输出也不是当前最大问题。真正的问题是 Level 63 只有 `1053` 生命、`1180` EHP，而且冰抗和电抗严重不合格。现在不是先追伤害的时候，必须先补生命和抗性。

## 当前公开面板

```text
等级：63
职业：Martial Artist
生命：1053
能量护盾：0
魔力：576
Spirit：46
EHP：1180
移动速度：122%

护甲：472
闪避：380
格挡：14%

火抗：28%
冰抗：-13%
电抗：-46%
混沌抗：15%

最低最大承伤：729
```

这个面板说明一件事：角色不是“差一点无敌”，而是防御地板还没搭起来。特别是 `-46%` 电抗，已经是 build-breaking 级别的问题。

## 当前技能壳

主轴大概是：

```text
Storm Wave
  Elemental Armament II
  Shock
  Branching Fissures I

Hollow Form
  Whirling Assault
  Heavy Swing
  Heft

Tempest Bell
  Magnified Area I
  Rage I
```

其他技能还包括：

```text
Ice Strike
Glacial Cascade
Frozen Locus
Siphoning Strike
Falling Thunder
Charge Regulation
Hollow Focus
```

技能方向不算乱到不能救。`Storm Wave` 作为主输出，`Elemental Armament II + Shock + Branching Fissures I` 是合理的清图/闪电攻击方向。问题是技能再合理，也撑不住负电抗和低生命。

## 做对了什么

### 1. 主输出方向清楚

`Storm Wave` 是当前角色最像主轴的技能。它有元素攻击、感电、范围分裂的支援组合，说明不是随便乱插。

### 2. 鞋子很好，先别动

```text
Entropy March, Steeltoe Boots
  25% Movement Speed
  +94 maximum Life
  Reduced Shock duration
```

这双鞋很适合当前阶段。它有跑速、有生命，还帮忙处理一点感电压力。短期不用换。

### 3. 项链也可以先保留

```text
Plague Charm, Pearlescent Amulet
  +9% all elemental resistance implicit
  +46 Spirit
  +12 all attributes
  +15% Chaos Resistance
  mana / mana regen
```

这条项链给 Spirit、全抗、混沌抗、属性和魔力，功能很多。虽然不是终局神装，但不是当前最大短板。

### 4. 武器够用，不是第一修车点

```text
Brood Song, Guardian Quarterstaff
  physical damage
  added fire damage
  critical chance
  critical damage
  attack speed
```

这把杖有攻击速度、暴击和附加火伤。它可以继续支撑当前阶段，不需要第一时间换。

## 最大问题

### 1. 电抗是全车最大洞

```text
Lightning Resistance: -46%
```

这是最危险的问题。很多玩家会误判为“输出不够”或者“操作不行”，但这里公开面板很清楚：角色遇到电伤很容易直接蒸发。

短期目标：

```text
电抗先变成正数
然后尽快拉到 40%+
之后再往 60% / 75% 靠
```

### 2. 冰抗也是负数

```text
Cold Resistance: -13%
```

冰抗负数会让冰系伤害、冻结压力、冰地板类场景都变得很难受。它不是电抗那么夸张，但也必须修。

短期目标：

```text
冰抗至少拉到 30%+
更好是 50%+
```

### 3. 生命太低

```text
Life: 1053
EHP: 1180
```

Level 63 这个血量偏低。如果目标是“无敌”，这不是可接受地板。

短期目标：

```text
生命先到 1500+
EHP 先到 2000+
```

### 4. 太多装备槽没有承担生存责任

当前角色用了好几个有趣但不保命的装备：

```text
Birthright Buckle, Wide Belt
  有功能性，但没有生命和抗性

Lochtonial Caress, Fists of Stone
  有攻速和充能味道，但没有生命和抗性

Cracklecreep, Ruby Ring
  火伤 / 点燃扩散，但没有生命和冰电抗

Blistering Bond, Ruby Ring
  有生命和火抗，但倒扣冰抗

Dread Jack, Full Plate
  有护甲机制，但没有生命和抗性

Havoc Keep, Visored Helm
  有命中、魔力和冰抗，但没有生命
```

这些装备单看都有理由，但拼在一起就把角色的生命和抗性掏空了。

## 修车优先级

### 第一优先级：换戒指

先换掉 `Cracklecreep Ruby Ring`。

它现在给的是火伤和点燃扩散，但没有生命、没有冰抗、没有电抗。对于这台车来说，它的机会成本太高。

目标戒指：

```text
+50 maximum Life
+30% Lightning Resistance
+20% Cold Resistance
可选：Fire Resistance / Mana / Attributes / Elemental Damage with Attacks
```

如果换完以后冰抗还是很低，再考虑把 `Blistering Bond` 也换掉。`Blistering Bond` 至少有生命，但它倒扣冰抗，所以不是长期舒适装备。

### 第二优先级：换腰带

`Birthright Buckle` 现在不解决核心问题。腰带通常是便宜补生命和抗性的好位置。

目标腰带：

```text
+70 maximum Life
+30% Lightning Resistance
+20% Cold or Fire Resistance
可选：Charm 相关词缀 / Flask 相关词缀
```

如果预算有限，腰带和戒指通常是最容易把电抗从负数救回来的地方。

### 第三优先级：换手套

`Lochtonial Caress` 有攻速和充能价值，但没有生命抗性。如果这个 build 不是强依赖它产球，就应该换。

目标手套：

```text
+50 maximum Life
+30% Lightning Resistance
+20% Cold Resistance
可选：Attack Speed
```

如果本人非常喜欢 Lochtonial 的手感，可以晚一点换，但要知道这就是在用防御换功能。

### 第四优先级：换胸甲

当前胸甲没有生命和抗性。Level 63 的胸甲槽应该承担更大防御责任。

目标胸甲：

```text
+100 maximum Life
+30% Lightning Resistance
+20% Cold or Fire Resistance
Armour / Evasion / Energy Shield 随底子自然补
```

这一步会明显提升 EHP。

### 第五优先级：换头盔

当前头盔不是完全没用，但没有生命。等戒指、腰带、手套处理后，头盔也要补。

目标头盔：

```text
+60 maximum Life
+30% Lightning Resistance
+20% Cold or Fire Resistance
可选：Accuracy / Mana / Critical Chance
```

## 不建议现在做的事

### 不建议先换武器

武器不是当前最大问题。换武器可能让伤害变好看，但抗性和生命不修，还是会死。

### 不建议先抠输出支援

`Storm Wave` 的主支援目前能用。现在改几个支援宝石，解决不了 `-46%` 电抗。

### 不建议继续堆有趣 unique

这台车现在的问题不是缺花活，是缺基础盘。Unique 可以以后再玩，当前阶段先让黄装把生命和抗性补起来。

## 最低购物过滤器

如果去市场淘宝，先按下面这种思路搜。

### 戒指

```text
非 unique
需求等级 <= 当前等级
+50 maximum Life
+30% Lightning Resistance
+20% Cold Resistance
价格：先看 1 exalt / 2 exalt 档
```

### 腰带

```text
非 unique
+70 maximum Life
+30% Lightning Resistance
+20% Cold or Fire Resistance
价格：先看 1 exalt / 2 exalt 档
```

### 手套

```text
非 unique
+50 maximum Life
+30% Lightning Resistance
+20% Cold Resistance
可选：Attack Speed
价格：先看 1 exalt / 2 exalt 档
```

### 胸甲

```text
非 unique
+100 maximum Life
+30% Lightning Resistance
+20% Cold or Fire Resistance
价格：先看 1-3 exalt 档
```

## 修完以后应该长什么样

短期合格线：

```text
Life: 1500+
EHP: 2000+
Fire Resistance: 50%+
Cold Resistance: 40%+
Lightning Resistance: 40%+
```

舒服线：

```text
Life: 1800+
EHP: 2500+
三元素抗性接近 75%
```

到这个时候，再回头调输出、珠宝、支援、技能取舍，才比较有意义。

## 最终结论

这不是废 build。它有主轴，有输出技能，有能继续用的鞋子、项链和武器。

真正的问题是装备槽之间没有形成防御系统。太多位置在提供“有趣效果”，但没有提供生命和抗性。对 Level 63 来说，当前最优修车不是重做整套 build，而是立刻用稀有黄装把生命、电抗、冰抗补起来。

人话版本：

```text
发动机能响。
方向盘也能打。
但是车门没关，窗户漏风，底盘没焊牢。

先补电抗和血量。
别先追伤害。
```
