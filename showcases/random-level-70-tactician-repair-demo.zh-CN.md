# 随机 Level 70 Tactician 修车 Demo

日期：2026-05-30

来源角色：

- 角色：`SexySchoolGirlxz`
- 账号：`Vladilena_-6547`
- 联盟：`Runes of Aldur`
- 职业：`Tactician`
- 等级：`70`
- 公开页面：<https://poe.ninja/poe2/builds/runesofaldur/character/Vladilena_-6547/SexySchoolGirlxz>

## 真实性边界

这是一个基于 poe.ninja 公开角色数据的 build 修车 demo。

本报告使用的是公开角色 payload：防御面板、装备、技能连线、珠宝、天赋点数量和可见 build 结构。

这不是完整怪物伤害模拟。没有当前怪物数值、地图词缀、玩家操作、死亡记录时，我们做的是实战 triage，不是精算版生存数学。

## 一句话诊断

这个号不是坏车。它是一个能跑的 crossbow 元素 Tactician，输出路线很清楚，但 Level 70 阶段防御预算不够。

## 当前状态

核心身份：

```text
Crossbow Tactician
Stormblast Bolts / Galvanic Shards
Herald of Thunder 辅助壳
元素攻击 scaling
```

关键防御面板：

```text
生命：1321
能量护盾：64
有效生命池：2130
移动速度：111%
护甲：43
闪避：304
实际闪避率：3%
火抗：36%
冰抗：75%
电抗：54%
混沌抗：0%
最低最大承伤：1353
```

主要技能连线：

```text
Stormblast Bolts L14
  Elemental Armament II
  Ice Bite II
  Rapid Attacks I
  Close Combat I

Galvanic Shards L15
  Elemental Armament I
  Double Barrel III
  Fork
  Mobility

Mirage Archer L12
  Prolonged Duration I
  Explosive Shot
  Cooldown Recovery II

Herald of Thunder L13
  Elemental Armament I
  Elemental Focus
  Deadly Herald
```

## 做对了什么

攻击身份是成立的。这个角色明显是在走 crossbow 技能、元素攻击、Herald 伤害、projectile / attack tempo 的路线。

武器能用：

```text
Spirit Core Cannonade Crossbow
130% increased Physical Damage
附加物理伤害
crafted 冰伤
火 rune / 电 rune 附加伤害
Grenade Skills fire an additional Projectile
```

鞋子很适合推进：

```text
20% 移动速度
+103 生命
+39 魔力
+27% 火抗
+26% 电抗
电抗 rune
生命回复
```

衣服在做关键功能：

```text
Enfolding Dawn
+100 Spirit
+15% 全元素抗性
火抗 rune
```

## 主要问题

### 1. 火抗和电抗没有满

冰抗 `75%` 很好，但火抗只有 `36%`，电抗只有 `54%`。

Level 70 这个阶段，这就是第一优先级。角色平时清图可能看起来没事，但遇到错误的元素 hit 会突然暴毙。

修车目标：

```text
火抗：75%
电抗：75%
冰抗：保持满
混沌抗：后面再补，但不要在火电没满之前强追
```

### 2. 物理防御很薄

当前数据：

```text
护甲：43
闪避：304
实际闪避率：3%
物理最大承伤：1389
```

这说明角色主要靠击杀速度、走位、回复在跑。能玩，但不硬。

修车目标：

```text
尽量补生命。
优先找不会破坏抗性计划的护甲/闪避底子。
不要为了小输出牺牲元素抗性上限。
```

### 3. 珠宝有明显错配词缀

两个 rare Emerald 珠宝有 Herald 伤害，这是有用的；但也有 bow 和 poison 词缀：

```text
Luminous Bloom
  13% increased Accuracy Rating with Bows
  10% chance to Poison on Hit
  Herald Skills deal 25% increased Damage

Armageddon Hope
  7% increased Damage with Bows
  9% chance to Poison on Hit
  Herald Skills deal 24% increased Damage
  Debuffs expire 8% faster
```

这个角色用的是 crossbow，不是 bow。Herald 词缀有价值，但 bow 词缀基本是浪费预算。

更合适的珠宝目标：

```text
projectile damage
attack damage
elemental damage with attacks
lightning damage
attack speed
如果命中真的缺，再补 accuracy
能带 life / resistance 更好
```

## 修车顺序

第一优先级：

```text
补满火抗和电抗。
```

优先从戒指、项链、头、腰带、rune 上解决。主输出技能先不要乱动。

第二优先级：

```text
替换错配珠宝。
```

能保留 Herald damage 最好，但不要继续为 crossbow 角色支付 bow-only 词缀预算。

第三优先级：

```text
增加生命和真实减伤。
```

现在移动速度和输出壳能支撑推进，但防御数字偏低，进更难内容会开始露馅。

第四优先级：

```text
抗性地板稳了以后，再考虑武器升级。
```

当前 crossbow 够用。提升伤害当然好，但不应该排在防御修复之前。

## 最终结论

这是一个有明确思路的可用 build，不需要推倒重来。

正确修车方向是：

```text
保留 crossbow 元素攻击壳。
先补满火抗和电抗。
换掉 bow / poison 这种不服务 crossbow 的珠宝浪费。
补更多生命或真实防御。
之后再回头看武器伤害。
```

人话版本：发动机能跑，方向也对，但底盘太轻，先把抗性和生存补起来。
