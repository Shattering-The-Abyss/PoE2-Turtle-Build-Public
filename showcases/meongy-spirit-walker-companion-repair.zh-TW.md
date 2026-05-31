# Spirit Walker 夥伴召喚修車報告：Meongy

日期：2026-05-31

來源：

- 公開 poe.ninja PoB：<https://poe.ninja/poe2/pob/1c236>
- 角色等級：`65`
- 職業：`Huntress`
- 昇華：`Spirit Walker`

## 真實性邊界

這是基於公開 poe.ninja PoB 匯出的實戰修車報告。

本報告使用的是目前角色狀態：防禦面板、技能組、裝備，以及可見的 Spirit Walker 夥伴方向。它不是最終 meta BD，也不是完整傷害模擬。

## 一句話診斷

這個角色已經在正確路線上：`Huntress -> Spirit Walker -> companion / 烏龜生存路線`。方向不是錯的。主要問題是夥伴核心已經有了，但防禦和資源地板還沒完全追上。

## 目前狀態

```text
等級：65
職業：Huntress
昇華：Spirit Walker
生命：1499
能量護盾：26
Mana：620
Spirit：1
未保留 Spirit：0
有效生命池：2499
護甲：637
閃避：1438
格擋：26%
火抗：43%
冰抗：9%
電抗：-9%
混沌抗：7%
```

主要技能殼：

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

## 做對了什麼

這台車已經有真正的 companion 路線資產。

重要可保留裝備：

```text
項鍊：
  +99 maximum Life
  +2 to Level of all Minion Skills

頭盔：
  +99 maximum Life
  +2 to Level of all Minion Skills
  從 Evasion 獲得 Deflection

腰帶：
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

其中 `+2 minion` 項鍊和頭盔尤其重要。這是路線資產，不是隨便的練級垃圾裝。

## 主要問題

### 1. Spirit 太緊

目前面板：

```text
Spirit: 1
Unreserved Spirit: 0
```

對 Spirit Walker companion 路線來說，這是最重要的資源警告。現在能跑，但幾乎沒有 Spirit 彈性。後面任何保留、光環、夥伴組合或輔助調整，都可能直接卡住。

這不代表目前配置錯了，而是後續升級必須盯緊 Spirit。

### 2. 冰抗和電抗不夠

目前抗性：

```text
Fire: 43%
Cold: 9%
Lightning: -9%
Chaos: 7%
```

火抗暫時還能看，冰抗和電抗不行。電抗是負數，是最大危險點。

短期目標：

```text
Lightning：先變正數，再往 75% 靠
Cold：先到 50%+，再往 75% 靠
Fire：繼續往 75% 靠
Chaos：至少保持非負
```

### 3. 鞋子是最明顯升級位

目前鞋子：

```text
Viper Hoof, Covered Sabatons
+78 Mana
+22% Cold Resistance
沒有生命
沒有移速
```

65 級還沒有移速和生命，代價太大。這是第一優先級替換位。

### 4. 手套也偏弱

目前手套：

```text
+29 maximum Life
+87 maximum Mana
+22 Intelligence
+178 Accuracy
```

臨時能用，但 Accuracy 不是 companion 路線核心。這個槽位應該承擔更多防禦工作。

### 5. 戒指還是過渡味

一個戒指火抗很多，但沒血。另一個有全抗和智力，也沒血。能用，但後面應該變成補血、電抗、冰抗的槽位。

## 修車計畫

## 個人化 Loot Filter

下載：

- [Meongy Spirit Walker Level 65 Loot Filter](../loot-filters/meongy-spirit-walker-level-65.filter)
- 合併後的 raw 下載連結：<https://raw.githubusercontent.com/Shattering-The-Abyss/PoE2-Turtle-Build-Public/main/loot-filters/meongy-spirit-walker-level-65.filter>

Filter 目的：

```text
使用 NeverSink 的 1-REGULAR PoE2 filter 作為底。
在 NeverSink 規則前面加一小段 Meongy 專屬 overlay。
高亮目前值得撿起來鑑定的修車槽位，同時保留 NeverSink 原本的通貨、寶石、底子和經濟規則。
```

重要限制：

```text
遊戲內 loot filter 不能檢查未鑑定詞綴，例如 +60 life 或 +25 lightning resistance。
它能做的是把目前最值得撿起來鑑定的物品類型高亮出來。
```

### 第一優先級：換鞋

找：

```text
20%+ Movement Speed
+60 maximum Life 或更高
+Lightning Resistance
+Cold or Fire Resistance
```

這是最高收益的即時修車點。

### 第二優先級：換手套

找：

```text
+60 maximum Life 或更高
兩個有用抗性
屬性或 Mana 是加分項
防禦底子是加分項
```

除非玩家目前手感特別依賴命中，否則不要為 attack accuracy 付溢價。

### 第三優先級：清戒指

找：

```text
+Life
+Lightning Resistance
+Cold Resistance or Fire Resistance
缺屬性 / Mana 可以順便補
```

目標不是花俏傷害，而是讓 companion 路線更安全。

### 第四優先級：以後再升級盾牌

目前盾牌作為低級抗性盾能用，但以後可以升級。

以後找：

```text
+Life
+Block
+兩個抗性
Armour/Evasion 或 Armour/ES 底子
如果便宜，帶 Spirit 更好
```

## 不要急著換

這些先留：

```text
+2 minion 項鍊
+2 minion 頭盔
有生命的胸甲
有生命 + 冰電抗的腰帶
```

這些不是完美裝，但它們支持目前真實方向。

## 最終結論

這是真正的 Spirit Walker companion 角色。方向應該保留。

人話版本：

```text
保留 +2 minion 頭和項鍊。
保留 companion 主線。
第一換鞋。
第二換手套。
用戒指修電抗和冰抗。
在加更多保留之前，持續盯 Spirit。
```

這台車不是因為計畫錯了才卡，而是防禦地板需要追上夥伴路線。
