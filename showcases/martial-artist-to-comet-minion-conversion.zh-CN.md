# Martial Artist 转召死彗星修车报告

日期：2026-05-31

来源：

- 公开 poe.ninja PoB：<https://poe.ninja/poe2/pob/1c1ef>
- 玩家提供的视频路线截图：`召唤物死亡时释放 -> 彗星`
- 被动洗点参考：<https://www.poe2wiki.net/wiki/Passive_skill_tree>

## 真实性边界

这是一份“能不能转、怎么转、值不值得转”的转换评估，不是完整成品 BD。

当前角色是 81 级 Monk / Martial Artist。目标路线来自视频截图，看起来是偏 Witch / Blood Mage 的召死彗星体系。下面会把当前角色硬数据和转换推断分开说。

## 一句话诊断

这不是小洗点。当前角色是 `Killing Palm / Quarterstaff / Attack / Crit` 武圣壳子；目标是 `Minion / Trigger / Spell / Spirit / Curse` 壳子。能转，但更像换发动机，不是调参数。

## 当前角色状态

```text
等级：81
职业：Monk
升华：Martial Artist
当前主技能：Killing Palm L12
当前武器：稀有 Sinister Quarterstaff
已点被动：114 点
```

关键面板：

```text
生命：1538
能量护盾：60
有效生命池：1647
护甲：27
闪避：201
火抗：27%
冰抗：4%
电抗：-18%
混沌抗：8%
Spirit：1
未保留 Spirit：-89
```

当前技能壳：

```text
Killing Palm L12
  Charge Profusion I
  Thrill of the Kill
  Blazing Critical

Pounce L3
  Rapid Attacks II
  Compressed Duration I

Lingering Illusion L13
  Prolonged Duration I

Charge Regulation L14
Wind Dancer L14
```

## 目标路线从截图读到什么

视频截图的核心大概是：

```text
召唤恶狼 / 狼群
召唤物死亡时释放
彗星
冷酷之宴
共鸣之盾
元素要害
寒霜爆
如果走蓝量版，可能还带大法师
```

截图里还写了几个关键边界：

```text
狼召彗星需要约 120 Spirit
召唤契约要根据血量调配
如果狼血量偏低，用 1 级契约
狼必须只放在套装 1，否则可能卡不出复活 bug
```

## 武僧哪个升华适合？

如果一定要留在 Monk：

```text
Invoker > Acolyte of Chayula > Martial Artist
```

### Invoker

Invoker 是最不别扭的 Monk 选择。它和元素、法术、资源、防御的关系更接近召死彗星的需求。如果坚持用武僧转，这个优先测。

### Acolyte of Chayula

不作为第一推荐。它更偏 chaos / darkness / 资源机制，可能能玩出东西，但不是召死彗星最干净的壳子。

### Martial Artist

当前 Martial Artist 最不适合继续硬撑。这个角色已经明显是攻击身份：Killing Palm、quarterstaff、暴击、近战路径。把 Martial Artist 留着去玩召死彗星，会浪费太多升华价值。

## 最适合目标路线的职业

如果问“这条视频路线最适合谁”，答案大概率不是 Monk。

截图路线更像：

```text
Witch / Blood Mage
```

Blood Mage 天然更接近生命、法术成本、残留、生存资源、召唤/触发这些主题。Monk 能改，但属于改装车。

## 洗点金币估算

当前角色：

```text
已点被动：114 点
```

81 级洗点成本按 wiki 表约：

```text
3089 gold / 点
```

粗算：

```text
小修 30 点：约 92,670 gold
中修 60 点：约 185,340 gold
大修 90 点：约 278,010 gold
全洗 114 点：约 352,146 gold
```

这次不是 30 点小修。合理预算：

```text
最低：300k gold
舒服：400k+ gold
包含试错：500k+ gold
```

如果当前版本不能轻松换升华类别，那成本和风险还要再往上算。

## 哪些装备可以暂留

### 可以先用

头盔：

```text
Hate Star, Tribal Mask
  +166 maximum Life
  +79 maximum Mana
  +33% Cold Resistance
```

不完美，但有血有蓝，能临时用。

Ruby Ring：

```text
Behemoth Spiral
  +54 maximum Life
  +11% all Elemental Resistances
  +28% Fire Resistance
  +22% Lightning Resistance
```

这个戒指可以当过渡装。

Amethyst Ring：

```text
Golem Grasp
  +49 maximum Life
  +12 all Attributes
  +8% Chaos Resistance implicit
```

有血和属性，但攻击伤害、物理攻击偷蓝这些词缀转流派后价值下降。

## 哪些必须换

### 武器

当前 `Sinister Quarterstaff` 是攻击武器，不属于目标体系。

根据参考视频路线，这里不应该说成“买 Spirit 武器”，也不应该默认换成 sceptre。更准确的目标武器身份是：

```text
主手：法杖
副手：盾牌
```

法杖负责法术输出侧：

```text
法术伤害
法术等级 / 冰法术等级，如果有
施法速度
如果最终走暴击，找法术暴击相关
如果走大法师，要蓝量
```

盾牌负责生存侧：

```text
生命
抗性
格挡 / 防御价值
能量护盾或护甲/能盾底子
如果市场和底子允许，可以顺带带 Spirit
```

Spirit 仍然是必须解决的预算，但它应该作为整套 build 的资源方案来解决：天赋、项链、胸甲、盾牌和其他装备一起凑。不能默认“武器位必须是 Spirit 武器”。

### 项链

当前项链有：

```text
+1 to Level of all Melee Skills
```

这对召死彗星基本不对路。要换成：

```text
+Spirit
+法术 / 召唤相关等级或伤害
+生命
+抗性
+缺属性就补属性
```

### 空装备槽

当前 PoB 里这些位置是空的：

```text
胸甲
手套
鞋子
```

这是转换前的大问题。这些槽位必须用来补生命、抗性、Spirit/资源、防御。

### 抗性

当前抗性还不能转：

```text
火抗：27%
冰抗：4%
电抗：-18%
混沌抗：8%
```

转换前至少要做到：

```text
三元素抗接近 75%
优先修电抗
混沌抗至少非负
```

## 转换前准备清单

花金币前先准备：

```text
1. 确认 Monk 升华能不能顺利换。
2. 准备至少 300k-400k gold。
3. 准备目标技能宝石。
4. 准备目标支援宝石。
5. 做出 120 Spirit 方案，但不要默认武器必须是 Spirit 武器。
6. 补齐胸甲、手套、鞋子。
7. 先修电抗。
8. 在 PoB 里模拟新树，确认 Spirit 不是负数。
9. 认真判断是否不如重练 Witch / Blood Mage。
```

## 实战建议

如果只是想保留武僧身份，体验视频机制：

```text
能换就往 Invoker 转。
不要继续用 Martial Artist 当最终壳子。
准备 400k+ gold。
先买法杖、防御盾牌、Spirit 方案组件和抗性装备。
技能包凑齐后再洗树。
```

如果想要最干净、最接近视频的版本：

```text
重练 Witch / Blood Mage。
```

## 最终结论

能转，但贵，而且结构别扭。

人话版本：当前 Martial Artist 是近战攻击车，目标召死彗星是法术触发发动机。你可以把发动机焊进去，但如果目标是按视频舒服跑，Blood Mage 车架大概率更合适。
