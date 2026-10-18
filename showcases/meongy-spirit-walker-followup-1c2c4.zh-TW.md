# Spirit Walker 夥伴召喚後續報告：Meongy 1c2c4

日期：2026-05-31

來源：

- 更新後的 poe.ninja PoB：<https://poe.ninja/poe2/pob/1c2c4>
- 原始修車報告：[Meongy Spirit Walker 夥伴召喚修車報告](meongy-spirit-walker-companion-repair.zh-TW.md)

## 真實性邊界

這是針對更新後角色狀態的後續報告。

它不替代原始報告。原始報告定位的是緊急修車優先級；這份報告檢查她改了什麼，以及下一層修車應該往哪裡走。

## 一句話診斷

這次更新是一次很成功的修車。

角色修掉了最危險的問題：電抗不再是負數，鞋子修好了，手套修好了，Spirit 不再完全卡死，而且裝備上已經有更多真正支援 companion 路線的東西。

下一個問題已經不是「這車壞了」。現在的問題是收束優化：繼續抬高防禦地板，換掉低價值戒指和盾牌，同時在強化 companion 體系時保留 Spirit 彈性。

## 快照對比

原始報告：

```text
等級：65
生命：1499
能量護盾：26
Spirit：1
未保留 Spirit：0
火抗：43%
冰抗：9%
電抗：-9%
混沌抗：7%
```

更新後 1c2c4：

```text
等級：71
生命：1696
能量護盾：185
Mana：681
Spirit：100
未保留 Spirit：19
護甲：546
閃避：1590
閃避率：15%
格擋：0%
火抗：56%
冰抗：44%
電抗：74%
混沌抗：28%
```

改善點：

```text
生命：+197
能量護盾：+159
電抗：-9% -> 74%
冰抗：9% -> 44%
火抗：43% -> 56%
混沌抗：7% -> 28%
Spirit 彈性：0 未保留 -> 19 未保留
```

這是實質修車，不是表面變化。

## 目前技能殼

主要 companion 組合：

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

判斷：

```text
這現在更明顯是一隻 Spirit Walker companion 角色。
它不再只是借用 companion 工具。
武器和技能組已經開始直接支援這條路線。
```

## 她修對了什麼

### 1. 鞋子修好了

新鞋：

```text
Vengeance Stride, Bastion Sabatons
20% increased Movement Speed
+85 maximum Life
+39 maximum Mana
+27% Cold Resistance
+27% Lightning Resistance
Rune/enchant 額外給 Lightning Resistance、Life、Mana
```

結論：

```text
非常好的修車。
這正是原始報告想要的鞋子方向。
除非出現明顯升級，否則保留。
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
Rune/enchant 額外給 Cold Resistance、Life、Mana
```

結論：

```text
非常好的修車。
這個槽位已經從弱填充變成真正的防禦支點。
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

結論：

```text
這是貨真價實的 Spirit Walker / companion 路線裝備。
它解決了之前 Spirit 卡死的問題，並且給了直接的 minion / ally scaling。
除非出現非常貴且明顯更強的版本，否則保留。
```

### 4. companion 傷害武器也是真的

另一把長矛：

```text
Dire Edge, Branched Spear
Companions deal 50% increased Damage
48% increased Damage while your Companion is in your Presence
Physical damage and life/mana on kill
```

結論：

```text
這是路線相關裝備，不是隨機傷害。
現在裝備上已經有真正的 companion scaling。
```

## 剩餘問題

### 1. 冰抗和火抗變好了，但還沒完成

目前抗性：

```text
Fire: 56%
Cold: 44%
Lightning: 74%
Chaos: 28%
```

電抗在這個階段基本修好了。

冰抗仍然是最弱的元素抗。火抗能玩，但也應該繼續往上補。

下一目標：

```text
Cold: 往 75% 推
Fire: 往 75% 推
Lightning: 保持接近上限
Chaos: 保持正數，後面再慢慢補
```

### 2. 戒指現在是最明顯升級區

目前戒指：

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

結論：

```text
戒指幫忙解決了一部分抗性壓力，但兩個都沒有生命。
現在鞋子和手套已經修好，戒指應該成為下一輪購買或製作目標。
```

理想戒指形狀：

```text
+Life
+Cold Resistance
+Fire Resistance or all Elemental Resistances
Attributes or Mana if needed
Chaos Resistance as bonus
```

現在不要為戒指上的傷害詞綴多花錢。

### 3. 盾牌偏弱

目前盾牌：

```text
Carrion Bastion, Crescent Targe
+13 maximum Life
+8% Fire Resistance
+7% Chaos Resistance
Raise Shield
```

結論：

```text
這現在是可見裝備裡最弱的槽位之一。
它還能用，只是因為其他裝備已經把角色救起來了。
戒指之後升級；如果市場上有便宜且明顯更好的盾牌，也可以提前換。
```

好盾牌目標：

```text
+60 maximum Life or better
Two useful resistances, preferably Cold + Fire
Block or defensive base value
Spirit only if available cheaply
```

### 4. Spirit 變好了，但仍然偏緊

目前：

```text
Spirit: 100
Unreserved Spirit: 19
```

這比之前好很多，但還不算寬裕。

後續任何 companion 組合、光環、保留或輔助調整，都應該先檢查 Spirit 再決定。

## 更新後的修車優先級

### 優先級 1：帶生命和冰抗的戒指

最實際的下一步，是找一枚能補 Life 和 Cold Resistance，同時不破壞 Lightning 的戒指。

搜尋目標：

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

### 優先級 2：第二枚戒指或盾牌，看價格

如果戒指便宜，先修兩枚戒指。

如果盾牌明顯便宜，第二枚戒指之前先換盾也可以。

盾牌搜尋目標：

```text
Shield
Required Level <= 71
+60 maximum Life or better
+25% Cold Resistance or better
+25% Fire Resistance or all Elemental Resistances
Block or good defensive base as bonus
```

### 優先級 3：保留 minion 等級裝備

不要隨便換掉：

```text
+2 minion helmet
+2 minion amulet
Spirit/minion sceptre
companion damage spear
fixed boots
fixed gloves
```

這些是 build identity 裝備，或者高價值修車成果。

### 優先級 4：最後才追傷害

傷害不是現在的緊急問題。

角色已經有：

```text
+2 minion helmet
+2 minion amulet
+2 minion sceptre
companion damage weapon/rune support
minion/companion jewels
```

下一步升級應該先讓角色更穩、更順。

## 更新後的個人化 Filter 說明

目前個人化 filter 已經改成以 NeverSink 的 1-REGULAR PoE2 filter 為底：

- [Meongy Spirit Walker Level 65 Loot Filter](../loot-filters/meongy-spirit-walker-level-65.filter)

但這次更新後，最重要的高亮槽位變成：

```text
Rings
Shields
Jewels
Charms
Currency
```

Meongy 專屬 overlay 放在 NeverSink 主體之前，所以這些修車槽位會額外醒目，同時保留 NeverSink 原本的通貨、寶石、底子和經濟規則。

鞋子和手套仍然輕度高亮，但已經不再緊急，因為目前鞋子和手套都很好。

## 最終結論

這是一次成功修車。

人話版：

```text
保留新鞋子。
保留新手套。
保留 +2 minion 頭和項鍊。
保留 Spirit/minion sceptre。
保留 companion damage 武器。
下一步先修戒指，再修盾牌。
冰抗和生命是下一階段最實際目標。
防禦地板更乾淨前，不要重金追傷害。
```

原始診斷被這次更新驗證了：方向是對的，地板是不夠的。裝備地板一抬起來，整個角色馬上變得清晰很多。
