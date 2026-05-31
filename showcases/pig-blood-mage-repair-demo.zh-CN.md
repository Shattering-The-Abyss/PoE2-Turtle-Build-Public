# Blood Mage 修车 Demo

日期：2026-05-30

来源：

- 来自玩家提供的 Path of Building 导出。
- 角色等级：`53`
- 职业：`Witch`
- 升华：`Blood Mage`

## 真实性边界

这是基于 PoB 导出的实战修车报告。

本报告使用的是导出里的角色状态：防御面板、技能组、装备、珠宝和武器组配置。

这不是完整怪物伤害模拟。这里做的是 triage：先修最明显、最容易导致 build 失效的问题，再回头看输出优化。

## 一句话诊断

这个角色有想法：Blood Mage、Minion Death 触发、Comet、Wolf Pack、法术 / 暴击 scaling。问题不是没脑洞，而是防御地板和资源结构还撑不起这个脑洞。

## 当前状态

```text
等级：53
职业：Witch
升华：Blood Mage
主想法：Cast on Minion Death -> Comet
辅助想法：Wolf Pack / Minion Instability / Elemental Weakness / Life Remnants
```

关键面板：

```text
生命：870
有效生命池：1063
护甲：170
闪避：156
火抗：45%
冰抗：55%
电抗：-18%
混沌抗：0%
Spirit：50
未保留 Spirit：-65
```

主要技能壳：

```text
Cast on Minion Death L10
  Comet L13
  Spell Cascade
  Boundless Energy II
  Energy Retention

Resonating Shield L5
  Minion Pact II
  Steadfast II

Elemental Weakness L12
  Heightened Curse
  Prolonged Duration II

Wolf Pack L13
  Minion Instability

Grim Feast L10
Life Remnants L13
Sigil of Power L8
```

## 做对了什么

这个 build 是有明确方向的。

`Cast on Minion Death -> Comet` 是一个真实的引擎想法。`Wolf Pack` 和 `Minion Instability` 指向用召唤物身体当触发 / 爆炸层。`Elemental Weakness` 支持法术输出，`Life Remnants` / `Grim Feast` 也符合 Blood Mage 的生存主题。

装备里也有一些有用部件：

```text
Rattling Sceptre
  +125 Spirit
  +1 to Level of all Minion Skills
  Grants Skeletal Warrior

Sire of Shards
  104% increased Spell Damage
  16% increased Cast Speed
  Spells fire 4 additional Projectiles

Shield
  +56 Life
  Fire Resistance
  Cold Resistance
  Stun Threshold
```

问题是这些部件在把角色往不同方向拉。

## 主要问题

### 1. 电抗是 build-breaking 级别的问题

当前电抗：

```text
Lightning Resistance: -18%
```

Level 53 这个阶段，这是第一修车目标。这不是小优化，而是会导致突然暴毙的大洞。

修车目标：

```text
电抗：至少 50%+
理想：75%
```

### 2. Blood Mage 生命太低

当前生命：

```text
Life: 870
```

对一个使用高成本触发 / 法术壳的 Blood Mage 来说偏低。导出里还显示生命成本压力：

```text
Life Cost: 73
Life per Second Cost: 41.9
```

也就是说角色一边输出一边扣自己的血，同时还要吃怪物伤害。低生命加负电抗，很容易还没开始表演，人先没了。

修车目标：

```text
生命：下一步先拉到 1100-1300+
```

### 3. Spirit / 武器组逻辑不稳定

导出显示：

```text
Spirit: 50
Unreserved Spirit: -65
```

这说明当前选择的配置撑不起想开的保留 / 召唤物，或者 PoB 的 active weapon set 和实际玩法没有对齐。

现在有两个互相竞争的武器身份：

```text
Sceptre + Shield:
  Spirit 更多
  +minion skill level
  Skeletal Warrior
  防御姿态更稳

Sire of Shards:
  法术 projectile 幻想更强
  额外 projectile
  但 minion / Spirit 稳定性更差
```

在资源数学成立之前，不建议两个方向同时贪。

### 4. 鞋子和头盔过旧

鞋子：

```text
10% Movement Speed
+20 Mana
+10% Cold Resistance
+13% Lightning Resistance
```

Level 53 还穿这个太弱。它没有解决电抗问题，没有生命，移速也低。

头盔：

```text
+41 Accuracy
Item Rarity
Critical Hit Chance
+11% Fire Resistance
```

Accuracy 对这个法术 / 召唤 / 触发壳基本浪费。这个装备位应该负责生命和抗性。

### 5. 珠宝有方向，但不是急救点

当前珠宝有 spell crit、crit damage、ignite magnitude，还有一条 plant damage。

这些不是现在最紧急的问题。它们可能服务法术暴击路线，但在电抗、生命、Spirit 修好之前，不该优先调珠宝。

## 修车顺序

### 第一优先级：换鞋

找：

```text
20%+ Movement Speed
+60 Life 以上
+25% Lightning Resistance 以上
任意第二抗性
```

这大概率是单件收益最高的修车点。

### 第二优先级：换头

找：

```text
+Life
+Lightning Resistance
+Fire or Cold Resistance
Energy Shield 或 Armour/Energy Shield 底子都可以
```

不要为这个 build 的 accuracy 付钱。

### 第三优先级：确定主武器身份

如果主路线是 minion-trigger Blood Mage：

```text
暂时优先 sceptre + shield。
先稳定 Spirit。
保留 minion level 和盾牌防御价值。
```

如果主路线是 Sire of Shards Comet：

```text
那就要接受 Spirit / minion setup 需要围绕 staff 重做。
不要默认 sceptre 那套召唤资源还在。
```

当前建议：

```text
先用 sceptre + shield，直到防御和 Spirit 地板修好。
Sire of Shards 先当一个很有潜力的输出玩具，不要马上当根基。
```

### 第四优先级：地板稳了再看输出

等角色做到：

```text
电抗接近满
火 / 冰抗往满抗靠
生命 1100-1300+
Spirit 不再是负预算
```

再去调：

```text
Comet support
spell crit jewel
minion death trigger uptime
Sire of Shards swap plan
```

## 最终结论

这不是废 build。它是一个很有意思的 build，但现在想法跑在车架前面了。

正确修车方向是：

```text
补电抗。
补生命。
修 Spirit。
确定一个主武器身份。
然后再优化 Comet / 暴击 / minion death scaling。
```

人话版本：烟花方案是真的，但先把轮胎和刹车装好，再继续加火药。
