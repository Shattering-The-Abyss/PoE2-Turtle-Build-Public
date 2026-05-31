# Blood Mage 修車 Demo

日期：2026-05-30

來源：

- 來自玩家提供的 Path of Building 匯出。
- 角色等級：`53`
- 職業：`Witch`
- 昇華：`Blood Mage`

## 真實性邊界

這是基於 PoB 匯出的實戰修車報告。

本報告使用的是匯出裡的角色狀態：防禦面板、技能組、裝備、珠寶和武器組配置。

這不是完整怪物傷害模擬。這裡做的是 triage：先修最明顯、最容易導致 build 失效的問題，再回頭看輸出最佳化。

## 一句話診斷

這個角色有想法：Blood Mage、Minion Death 觸發、Comet、Wolf Pack、法術 / 暴擊 scaling。問題不是沒腦洞，而是防禦地板和資源結構還撐不起這個腦洞。

## 目前狀態

```text
等級：53
職業：Witch
昇華：Blood Mage
主想法：Cast on Minion Death -> Comet
輔助想法：Wolf Pack / Minion Instability / Elemental Weakness / Life Remnants
```

關鍵面板：

```text
生命：870
有效生命池：1063
護甲：170
閃避：156
火抗：45%
冰抗：55%
電抗：-18%
混沌抗：0%
Spirit：50
未保留 Spirit：-65
```

主要技能殼：

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

## 做對了什麼

這個 build 是有明確方向的。

`Cast on Minion Death -> Comet` 是一個真實的引擎想法。`Wolf Pack` 和 `Minion Instability` 指向用召喚物身體當觸發 / 爆炸層。`Elemental Weakness` 支援法術輸出，`Life Remnants` / `Grim Feast` 也符合 Blood Mage 的生存主題。

裝備裡也有一些有用部件：

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

問題是這些部件在把角色往不同方向拉。

## 主要問題

### 1. 電抗是 build-breaking 級別的問題

目前電抗：

```text
Lightning Resistance: -18%
```

Level 53 這個階段，這是第一修車目標。這不是小最佳化，而是會導致突然暴斃的大洞。

修車目標：

```text
電抗：至少 50%+
理想：75%
```

### 2. Blood Mage 生命太低

目前生命：

```text
Life: 870
```

對一個使用高成本觸發 / 法術殼的 Blood Mage 來說偏低。匯出裡還顯示生命成本壓力：

```text
Life Cost: 73
Life per Second Cost: 41.9
```

也就是說角色一邊輸出一邊扣自己的血，同時還要吃怪物傷害。低生命加負電抗，很容易還沒開始表演，人先沒了。

修車目標：

```text
生命：下一步先拉到 1100-1300+
```

### 3. Spirit / 武器組邏輯不穩定

匯出顯示：

```text
Spirit: 50
Unreserved Spirit: -65
```

這說明目前選擇的配置撐不起想開的保留 / 召喚物，或者 PoB 的 active weapon set 和實際玩法沒有對齊。

現在有兩個互相競爭的武器身份：

```text
Sceptre + Shield:
  Spirit 更多
  +minion skill level
  Skeletal Warrior
  防禦姿態更穩

Sire of Shards:
  法術 projectile 幻想更強
  額外 projectile
  但 minion / Spirit 穩定性更差
```

在資源數學成立之前，不建議兩個方向同時貪。

### 4. 鞋子和頭盔過舊

鞋子：

```text
10% Movement Speed
+20 Mana
+10% Cold Resistance
+13% Lightning Resistance
```

Level 53 還穿這個太弱。它沒有解決電抗問題，沒有生命，移速也低。

頭盔：

```text
+41 Accuracy
Item Rarity
Critical Hit Chance
+11% Fire Resistance
```

Accuracy 對這個法術 / 召喚 / 觸發殼基本浪費。這個裝備位應該負責生命和抗性。

### 5. 珠寶有方向，但不是急救點

目前珠寶有 spell crit、crit damage、ignite magnitude，還有一條 plant damage。

這些不是現在最緊急的問題。它們可能服務法術暴擊路線，但在電抗、生命、Spirit 修好之前，不該優先調珠寶。

## 修車順序

### 第一優先級：換鞋

找：

```text
20%+ Movement Speed
+60 Life 以上
+25% Lightning Resistance 以上
任意第二抗性
```

這大概率是單件收益最高的修車點。

### 第二優先級：換頭

找：

```text
+Life
+Lightning Resistance
+Fire or Cold Resistance
Energy Shield 或 Armour/Energy Shield 底子都可以
```

不要為這個 build 的 accuracy 付錢。

### 第三優先級：確定主武器身份

如果主路線是 minion-trigger Blood Mage：

```text
暫時優先 sceptre + shield。
先穩定 Spirit。
保留 minion level 和盾牌防禦價值。
```

如果主路線是 Sire of Shards Comet：

```text
那就要接受 Spirit / minion setup 需要圍繞 staff 重做。
不要預設 sceptre 那套召喚資源還在。
```

目前建議：

```text
先用 sceptre + shield，直到防禦和 Spirit 地板修好。
Sire of Shards 先當一個很有潛力的輸出玩具，不要馬上當根基。
```

### 第四優先級：地板穩了再看輸出

等角色做到：

```text
電抗接近滿
火 / 冰抗往滿抗靠
生命 1100-1300+
Spirit 不再是負預算
```

再去調：

```text
Comet support
spell crit jewel
minion death trigger uptime
Sire of Shards swap plan
```

## 最終結論

這不是廢 build。它是一個很有意思的 build，但現在想法跑在車架前面了。

正確修車方向是：

```text
補電抗。
補生命。
修 Spirit。
確定一個主武器身份。
然後再最佳化 Comet / 暴擊 / minion death scaling。
```

人話版本：煙火方案是真的，但先把輪胎和煞車裝好，再繼續加火藥。
