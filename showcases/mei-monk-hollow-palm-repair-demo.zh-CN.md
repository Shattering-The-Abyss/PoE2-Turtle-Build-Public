# Hollow Palm Monk 修车 Demo

日期：2026-05-31

来源：

- 公开 poe.ninja 角色页：<https://poe.ninja/poe2/profile/1793653506-1046/runesofaldur/character/%E6%A2%85%E5%A4%A7%E5%B8%9D>
- 角色名：`梅大帝`
- 角色等级：`52`
- 职业：`Monk`
- 联赛：`Runes of Aldur`
- poe.ninja 模型数据更新时间：`2026-05-31T03:30:45Z`

## 真实性边界

这是基于公开 poe.ninja 角色页做的实战修车报告。

本报告使用的是公开角色状态：防御面板、技能组、装备、珠宝和核心 keystone。它不是完整怪物伤害模拟。这里做的是 triage：先修最容易导致角色暴毙的问题，再回头看输出优化。

## 一句话诊断

方向是对的：`Hollow Palm Technique` 加 `Storm Wave` 给了这个角色一个很清楚的空手闪电 Monk 身份。问题不是输出脑洞，而是防御地板太低，暂时撑不起“无敌”这个目标。

## 当前状态

```text
等级：52
职业：Monk
核心 Keystone：Hollow Palm Technique
主技能：Storm Wave L12
主技能支援：Elemental Armament II / Shock / Branching Fissures I
```

关键面板：

```text
生命：882
能量护盾：42
有效生命池：905
护甲：472
闪避：422
火抗：14%
冰抗：-9%
电抗：-41%
混沌抗：15%
最低最大承伤：663
```

主要技能壳：

```text
Storm Wave L12
  Elemental Armament II
  Shock
  Branching Fissures I

Tempest Bell L6
  Magnified Area I
  Rage I

Frozen Locus L12
  Rapid Attacks I
  Magnified Area I

Ice Strike L7
  Rapid Attacks I
  Elemental Armament I

Glacial Cascade L4
  Elemental Armament I
  Rapid Attacks I
```

## 做对了什么

这个 build 有一个能看懂的中心。

`Hollow Palm Technique` 要求双手空着，并让空手攻击可以像 quarterstaff 攻击一样使用。所以他不拿武器是对的，不是 bug。`Storm Wave` 这组也符合闪电攻击方向：`Elemental Armament II` 合理，`Shock` 合理，`Branching Fissures I` 帮清图。

装备里也有一些能用的东西：

```text
Entropy March, Steeltoe Boots
  25% Movement Speed
  +94 Life
  Stun Threshold
  Reduced Shock duration

Plague Charm, Pearlescent Amulet
  +9% all elemental resistance implicit
  +46 Spirit
  +12 all attributes
  +15% Chaos Resistance

Havoc Keep, Visored Helm
  Accuracy
  Mana
  Critical Hit Chance
  +17% Cold Resistance
```

问题是这些装备拼起来以后，还不是一个稳定的防御系统。

## 主要问题

### 1. 电抗是 build-breaking 级别的问题

当前电抗：

```text
Lightning Resistance: -41%
```

这是整台车最大的洞。面板最低最大承伤也是闪电：

```text
Lightning Maximum Hit Taken: 663
```

也就是说，哪怕主技能方向正确，遇到闪电伤害还是很容易突然暴毙。

修车目标：

```text
电抗：立刻往 75% 靠
短期目标：至少先变成正数，再拉到 50%+
```

### 2. 冰抗和火抗也不安全

当前元素抗性：

```text
Fire Resistance: 14%
Cold Resistance: -9%
Lightning Resistance: -41%
```

这不是“无敌”的地板。这是一个输出想法不错、但防御还没搭起来的练级角色。

修车目标：

```text
火抗：往 75% 靠
冰抗：往 75% 靠
电抗：最高优先级，往 75% 靠
```

### 3. 血量撑不起目标

当前生命：

```text
Life: 882
```

52 级还想打近战范围攻击，这个血量偏薄。如果目标是“无敌感”，这不是可接受地板。

修车目标：

```text
生命：下一步先到 1200+
舒服目标：后面到 1500+
```

### 4. 升华是 0 点

公开数据里显示：

```text
Ascendancy passive count: 0
```

如果还没做升华试炼，这就是一大块缺失强度。这个优先级比抠小词缀更高。

### 5. 有些装备槽没有承担足够生存责任

头盔：

```text
没有生命
只有 +17% 冰抗
命中和蓝量没有解决暴毙问题
```

戒指：

```text
Gold Ring 有打宝和蓝量，但没有提供足够血量 / 抗性
```

手套：

```text
有一些攻击向词缀，但没有生命，只有火抗
```

珠宝：

```text
4% Attack Speed 有用
Poison magnitude 对闪电 Storm Wave 路线基本不搭
```

## 修车顺序

### 第一优先级：修电抗

找装备时优先看：

```text
+Life
+Lightning Resistance
+Cold or Fire Resistance
```

最适合先修的槽位：

```text
戒指
头盔
腰带
手套
如果有明显升级，鞋子也可以
```

### 第二优先级：换掉低生存首饰

Gold Ring 现在没有承担足够防御工作。

找：

```text
+Life
+Lightning Resistance
+Cold Resistance or Fire Resistance
如果缺属性，可以带 attributes
```

角色还在死的时候，不要为了 rarity 付太多代价。

### 第三优先级：换头盔

找：

```text
+Life
+Lightning Resistance
+Cold or Fire Resistance
Evasion / Energy Shield 对 Hollow Palm 是加分项
```

对这个角色来说，一个朴素的防御头盔，比一个看起来聪明但不保命的头盔更值。

### 第四优先级：做升华

如果升华还没做，先做。

这不是小优化。0 点升华代表角色少了一大块职业身份和强度。

### 第五优先级：再调输出

等防御地板稳定以后，再看：

```text
Storm Wave support choices
Tempest Bell boss setup
Hollow Palm evasion / energy shield scaling
Attack speed
Lightning / elemental damage
Better jewel stats
```

## 最终结论

这不是废 build。它有清楚身份，核心技能组也能看懂。

正确修车路线是：

```text
保留 Hollow Palm。
保留 Storm Wave 主路线。
立刻修电抗。
然后修冰 / 火抗。
拉高生命。
完成升华。
最后再优化输出。
```

人话版本：发动机是真有想法，但底盘还没到“无敌”的标准。先把防御地板搭起来，再让闪电和尚开煮。
