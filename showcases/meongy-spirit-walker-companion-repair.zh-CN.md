# Spirit Walker 伙伴召唤修车报告：Meongy

日期：2026-05-31

来源：

- 公开 poe.ninja PoB：<https://poe.ninja/poe2/pob/1c236>
- 角色等级：`65`
- 职业：`Huntress`
- 升华：`Spirit Walker`

## 真实性边界

这是基于公开 poe.ninja PoB 导出的实战修车报告。

本报告使用的是当前角色状态：防御面板、技能组、装备，以及可见的 Spirit Walker 伙伴方向。它不是最终 meta BD，也不是完整伤害模拟。

## 一句话诊断

这个角色已经在正确路线上：`Huntress -> Spirit Walker -> companion / 乌龟生存路线`。方向不是错的。主要问题是伙伴核心已经有了，但防御和资源地板还没完全追上。

## 当前状态

```text
等级：65
职业：Huntress
升华：Spirit Walker
生命：1499
能量护盾：26
Mana：620
Spirit：1
未保留 Spirit：0
有效生命池：2499
护甲：637
闪避：1438
格挡：26%
火抗：43%
冰抗：9%
电抗：-9%
混沌抗：7%
```

主要技能壳：

```text
Companion: Diretusk Boar L12
  Feeding Frenzy I
  Hulking Minions I
  Rapid Attacks I

Twister L11
  Elemental Armament II
  Frost Nexus
  Retreat I

Whirling Slash L11
  Rapid Attacks I
  Cadence
  Rage I

Tame Beast L12
Barrage L10
Raise Shield
Spear Throw
```

## 做对了什么

这台车已经有真正的 companion 路线资产。

重要可保留装备：

```text
项链：
  +99 maximum Life
  +2 to Level of all Minion Skills

头盔：
  +99 maximum Life
  +2 to Level of all Minion Skills
  从 Evasion 获得 Deflection

腰带：
  +85 maximum Life
  +22% Cold Resistance
  +29% Lightning Resistance

胸甲：
  +127 maximum Life
  +20% Fire Resistance
  Armour/Evasion 底子

盾牌：
  +29 maximum Life
  +15% Fire Resistance
  +13% Cold Resistance
  +10% Lightning Resistance
```

其中 `+2 minion` 项链和头盔尤其重要。这是路线资产，不是随便的练级垃圾装。

## 主要问题

### 1. Spirit 太紧

当前面板：

```text
Spirit: 1
Unreserved Spirit: 0
```

对 Spirit Walker companion 路线来说，这是最重要的资源警告。现在能跑，但几乎没有 Spirit 弹性。后面任何保留、光环、伙伴组合或支援调整，都可能直接卡住。

这不代表当前配置错了，而是后续升级必须盯紧 Spirit。

### 2. 冰抗和电抗不够

当前抗性：

```text
Fire: 43%
Cold: 9%
Lightning: -9%
Chaos: 7%
```

火抗暂时还能看，冰抗和电抗不行。电抗是负数，是最大危险点。

短期目标：

```text
Lightning：先变正数，再往 75% 靠
Cold：先到 50%+，再往 75% 靠
Fire：继续往 75% 靠
Chaos：至少保持非负
```

### 3. 鞋子是最明显升级位

当前鞋子：

```text
Viper Hoof, Covered Sabatons
+78 Mana
+22% Cold Resistance
没有生命
没有移速
```

65 级还没有移速和生命，代价太大。这是第一优先级替换位。

### 4. 手套也偏弱

当前手套：

```text
+29 maximum Life
+87 maximum Mana
+22 Intelligence
+178 Accuracy
```

临时能用，但 Accuracy 不是 companion 路线核心。这个槽位应该承担更多防御工作。

### 5. 戒指还是过渡味

一个戒指火抗很多，但没血。另一个有全抗和智力，也没血。能用，但后面应该变成补血、电抗、冰抗的槽位。

## 修车计划

## 个性化 Loot Filter

下载：

- [Meongy Spirit Walker Level 65 Loot Filter](../loot-filters/meongy-spirit-walker-level-65.filter)
- 合并后的 raw 下载链接：<https://raw.githubusercontent.com/Shattering-The-Abyss/PoE2-Turtle-Build-Public/main/loot-filters/meongy-spirit-walker-level-65.filter>

Filter 目的：

```text
使用 NeverSink 的 1-REGULAR PoE2 filter 作为底。
在 NeverSink 规则前面加一小段 Meongy 专属 overlay。
高亮当前值得捡起来鉴定的修车槽位，同时保留 NeverSink 原本的通货、宝石、底子和经济规则。
```

重要限制：

```text
游戏内 loot filter 不能检查未鉴定词缀，例如 +60 life 或 +25 lightning resistance。
它能做的是把当前最值得捡起来鉴定的物品类型高亮出来。
```

### 第一优先级：换鞋

找：

```text
20%+ Movement Speed
+60 maximum Life 或更高
+Lightning Resistance
+Cold or Fire Resistance
```

这是最高收益的即时修车点。

### 第二优先级：换手套

找：

```text
+60 maximum Life 或更高
两个有用抗性
属性或 Mana 是加分项
防御底子是加分项
```

除非玩家当前手感特别依赖命中，否则不要为 attack accuracy 付溢价。

### 第三优先级：清戒指

找：

```text
+Life
+Lightning Resistance
+Cold Resistance or Fire Resistance
缺属性 / Mana 可以顺便补
```

目标不是花哨伤害，而是让 companion 路线更安全。

### 第四优先级：以后再升级盾牌

当前盾牌作为低级抗性盾能用，但以后可以升级。

以后找：

```text
+Life
+Block
+两个抗性
Armour/Evasion 或 Armour/ES 底子
如果便宜，带 Spirit 更好
```

## 不要急着换

这些先留：

```text
+2 minion 项链
+2 minion 头盔
有生命的胸甲
有生命 + 冰电抗的腰带
```

这些不是完美装，但它们支持当前真实方向。

## 最终结论

这是真正的 Spirit Walker companion 角色。方向应该保留。

人话版本：

```text
保留 +2 minion 头和项链。
保留 companion 主线。
第一换鞋。
第二换手套。
用戒指修电抗和冰抗。
在加更多保留之前，持续盯 Spirit。
```

这台车不是因为计划错了才卡，而是防御地板需要追上伙伴路线。
