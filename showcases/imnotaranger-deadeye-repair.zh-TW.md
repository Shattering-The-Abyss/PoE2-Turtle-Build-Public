# imnotaranger Deadeye 修車報告

來源：poe.ninja 公開角色模型，角色 `imnotaranger`，帳號 `nega_tive#4060`，Runes of Aldur。

本次快照：

- poe.ninja profile: <https://poe.ninja/poe2/profile/nega_tive-4060/runesofaldur/character/imnotaranger>
- poe.ninja 最後檢查時間：`2026-06-03T02:44:03Z`
- Level 68 `Deadeye`
- 主要技能殼：`Ice Shot`、`Tornado Shot`、`Snipe`、`Freezing Mark`
- 面板 DPS：`Ice Shot 9375`、`Tornado Shot 4559`、`Snipe 2799`
- Life: `1536`
- Energy Shield: `272`
- Mana: `530`
- Spirit: `139`
- Movement speed: `128%`
- 抗性：Fire `43`、Cold `38`、Lightning `70`、Chaos `0`
- 最低 maximum hit taken：Chaos `1672`
- Physical maximum hit taken：`1900`

這份報告只基於 poe.ninja 公開快照；沒有包含地圖錄影、死亡紀錄、倉庫預算或實際手感。

## Boss 傷害深挖結論

玩家回饋是：打一個 Boss 大概兩分鐘，過程像魂斗羅，角色沒傷害。

這個判斷可信。第一版報告抓到了防禦底盤問題，但這個 Boss 主訴會改變優先級：這不只是補抗性的小修，這套角色還需要傷害引擎大修。

目前 Boss 傷害警訊很具體：

- 主技能都是 `L14 Q0`。
- `Ice Shot` 只有 `9375` DPS。
- 本來應該負責瞄準爆發的 `Snipe` 只有 `2799` DPS。
- `Tornado Shot` 只有 `4559` DPS，而且目前更像覆蓋技能，不是 Boss payoff。
- 弓只有 `1.20` attacks per second，沒有 attack speed，沒有 crit scaling，flat elemental damage 也不夠高。
- rare ring、amulet、jewel、quiver 沒有一起承擔 Boss 傷害。
- `Polcirkeln` 對 chill / shatter 清圖身份有用，但它本身不是 Boss 擊殺引擎。

真實診斷是：

```text
清圖思路存在。
Boss 引擎不存在。
防禦底盤也太低，所以每個長 Boss 都會變成彈幕求生。
```

如果 Boss 打兩分鐘，所有防禦缺點都會被放大。角色不是單純因為脆才死，而是因為要脆很久。

## 簡短結論

這台車不是技能方向錯了。冷系弓投射物的想法是成立的：

```text
+1 projectile bow
Ice Shot 清圖
Tornado Shot 覆蓋
Snipe 嘗試單體爆發
Freezing Mark / Herald of Ice / Combat Frenzy 工具層
Polcirkeln 負責 chill -> shatter 轉換
```

真正的問題更簡單：

```text
輸出已經想開始刷圖，
但防禦底盤還停在劇情 / 早期地圖水平。
```

Level 68 時，火抗和冰抗沒滿，混沌抗是 0，chaos 和 physical 最大承傷都低於 `2000`。所以實戰會很隨機：有些怪能炸得很爽，但遇到強 rare、地面效果、混沌傷害或物理尖刺時，會在弓技能開始發揮之前直接倒。

第一步不是無腦買高級弓，但真正的大修必須包含傷害。只補抗性會讓兩分鐘 Boss 更安全，不會讓它變短。

## 現在能用的部分

### Bow

這把弓在目前階段夠用：

- `+1 to Level of all Projectile Skills`
- 附加 physical / fire damage
- increased elemental damage with attacks
- cold rune damage
- physical damage mana leech
- dexterity

這把弓不是廢品，但如果主訴是 Boss 時間，它大概率已經不夠了。

問題不是少一條詞綴，而是整個 Boss 畫像太弱：

```text
1.20 attacks per second
flat elemental damage 偏低
沒有 attack speed
沒有 critical strike scaling
沒有高端 elemental DPS
```

`+1 projectile skills` 很好，但不能單獨承擔 Boss 傷害。

### Body Armour

胸甲是目前比較好的裝備：

- `+198 maximum Life`
- fire / cold resistance
- energy shield
- life regeneration

除非新胸甲同時提升 life 和抗性，否則先保留。

### Helmet / Belt

頭和腰帶都有很高 life：

- Helmet: `+165 maximum Life`
- Belt: `+158 maximum Life`，3 charm slots

它們在撐底盤。可以以後升級，但不是第一輪亂換的對象。

### 冷系弓身份

技能包足夠清楚：

- `Ice Shot` 主清圖
- `Tornado Shot` 覆蓋
- `Snipe` 單點爆發嘗試
- `Freezing Mark`
- `Herald of Ice`
- `Combat Frenzy`
- `Wind Dancer`

這個身份可以繼續。修車目標是讓角色活到這套東西穩定運轉。

## 主要問題

### 0. 現在沒有真正的 Boss 擊殺方案

目前技能表分散在幾個攻擊上：

```text
Ice Shot L14 Q0      -> 清圖
Tornado Shot L14 Q0  -> 覆蓋
Snipe L14 Q0         -> 預期爆發，但面板很低
Barrage L14 Q0       -> 工具 / 冷卻包，不是可見傷害核心
```

清圖時這可能還行。打 Boss 時，build 需要一個明確答案：

```text
到底哪個按鈕負責殺 Boss？
```

現在答案不夠強。`Snipe` 沒扛起來，`Tornado Shot` 沒被做成 Boss payoff，`Ice Shot` 還帶著偏清圖的 `Fork`。

Boss 修車目標：

```text
先選定一個單體方案，
然後讓 bow / quiver / supports / jewels / jewelry 都服務這個方案。
```

### 1. 火抗和冰抗沒滿

目前：

```text
Fire      43 / 75
Cold      38 / 75
Lightning 70 / 75
Chaos      0 / 75
```

這是最優先修的問題。

大概需要補：

```text
Fire:      +32
Cold:      +37
Lightning: +5
Chaos:     能補多少補多少，第一目標 20-30
```

火冰沒滿之前，不建議投入明顯成本去買純傷害。

### 2. Boots 太薄

目前鞋子：

- 20% movement speed
- cold resistance
- reduced freeze duration
- 沒 life
- 沒第二條抗性

這是最乾淨的第一升級槽。

目標鞋子：

```text
25-30% movement speed
+maximum life
兩條有效抗性
可選 chaos resistance / evasion / freeze utility
```

如果一雙鞋能同時補 cold、fire、life，整台車會立刻穩很多。

### 3. Rare ring 更像練級戒指

目前 Topaz rare ring 給了一些 flat attack damage、dexterity、小 lightning resistance 和 life on kill。它沒有解決目前核心問題。

替換目標：

```text
高 fire 或 cold resistance
第二抗性或 chaos resistance
maximum life
如果買得起，再帶 flat elemental attack damage
dexterity 只在缺屬性時需要
```

Polcirkeln 可以先保留，因為它服務 chill / shatter 身份。rare ring 更適合先修。

### 4. Amulet 有 Spirit，但生存價值不足

項鍊給：

- `+39 Spirit`
- fire resistance
- evasion
- rarity

Spirit 有用，所以不能盲目換。但這個槽位沒有 life、沒有 cold resistance、沒有 chaos resistance，也沒有強到必須保留的傷害詞。

如果 reservation 不會壞，後續項鍊應該找：

```text
+Spirit
+maximum life
fire/cold/chaos resistance
projectile / attack / elemental / cold damage
```

### 5. Jewel 基本不在計畫內

目前 jewel：

- `5% increased Fire Damage`
- `16% increased Glory generation for Banner Skills`

對這套角色來說，這接近一顆死珠寶。

換成弓 / 冷 / 投射物珠寶：

```text
Projectile damage
Attack damage
Cold damage
Elemental damage with attacks
Critical damage / ailment / freeze value
maximum life or resistance if available
```

這是便宜、低風險、很乾淨的升級。

## 修車順序

### Phase 0：先讓 Boss 不再打兩分鐘

這是根據玩家回饋更新後的新優先級。

在買昂貴純防禦裝之前，先做這些：

1. 主技能寶石升級。`L14 Q0` 對想打 Boss 的角色來說太低。
2. 換掉目前 jewel。Fire damage + banner glory 基本不屬於這套 build。
3. 明確 Boss 按鈕：要麼把 `Snipe` 做成真正單體，要麼轉向 `Ice Shot` / `Barrage` 的 Boss 包。
4. 如果保留 `Fork` 清圖，就準備 Boss gem swap。`Fork` 是清圖 support，不應該當 Boss 答案。

### Phase 1：傷害和底盤一起修

目標：

```text
Life: 1700-1900+
Fire: 75
Cold: 75
Lightning: 75
Chaos: 20-30+
Movement speed: 盡量保住 25%+
Main damage skill: 更高 gem level，更合理 support，明確 Boss 方案
```

購買 / 製作順序：

1. Jewel：把 fire/banner 珠寶換成 bow/cold/projectile 方向。
2. Rare ring：替換 Topaz ring，補 life、缺失抗性，最好再帶 flat elemental attack damage。
3. Boots：movement speed + life + two resistances。
4. Quiver：預算允許時找 flat elemental damage、projectile damage、attack speed、crit value 或 accuracy。
5. Bow：預算允許時換更高 elemental DPS、attack speed、projectile skill level 的弓。

### Phase 2：真正重做 Boss 傷害

等角色有基本抗性、能站住以後：

1. 升級更高 elemental DPS、attack speed、projectile level 的弓。
2. 升級 quiver，找 flat elemental damage、projectile damage、attack speed、crit 或 accuracy。
3. Jewelry 從「隨機有用詞綴」改成「life/resist + attack damage」。
4. Support 圍繞真正 Boss 技能調整，不圍繞清圖。
5. 如果 `Snipe` 仍然打不過普通攻擊循環，就不要繼續把它當 Boss 方案。

## 槽位建議

### 先保留

- Bow：早期刷圖能用，但不是長期 Boss 武器。
- Body armour：life 和抗性不錯。
- Helmet：life 很好。
- Belt：life 很好，3 charm slots。
- Polcirkeln：服務 chill -> shatter 身份。

### 盡快替換

- Boots：需要 life 和更多抗性。
- Rare ring：需要真正的抗性 / life 價值，最好還帶 attack damage。
- Jewel：目前詞綴和 build 不匹配。
- Quiver：目前 flat damage 有用，但缺少這個槽位該提供的 Boss scaling。

### 謹慎替換

- Amulet：Spirit 有用，但長期看其餘詞綴不夠強。
- Gloves：fire/lightning 抗性和 life-on-kill 有用，但沒有 life。鞋子和戒指修完後，如果還脆，再看手套。

## 手動市場 Filter

### Boots

必須：

- `25%+ increased Movement Speed`
- `+# to maximum Life`
- fire / cold / lightning resistance 中的兩條

加分：

- chaos resistance
- evasion
- freeze / chill utility

### Ring

必須：

- `+# to maximum Life`
- 高 fire 或 cold resistance
- 第二抗性或 chaos resistance

加分：

- flat cold/fire/lightning damage to attacks
- attack speed
- dexterity
- accuracy

### Amulet

必須：

- 足夠 Spirit，保證 reservation 不壞
- maximum life 或明顯抗性價值

加分：

- projectile damage
- elemental damage with attacks
- cold damage
- attributes

### Jewel

必須：

- projectile / attack / cold / elemental attack damage

加分：

- critical damage
- freeze / ailment value
- maximum life
- resistance

### Bow

必須：

- 比目前弓高很多的 elemental DPS
- attack speed，或者總傷害畫像明顯更強
- 如果有預算，帶 projectile skill level

加分：

- flat cold damage
- flat lightning / fire damage
- critical strike chance / critical damage 方向
- accuracy / dexterity

### Quiver

必須：

- flat elemental damage to attacks
- projectile damage 或 attack speed

加分：

- critical damage / critical chance 方向
- accuracy
- dexterity
- resistance，如果它能避免其他槽位變成純防禦裝

## 最終建議

先做正確的大修：

```text
jewel -> rare ring -> boots -> quiver -> bow
```

目標是從：

```text
抗性沒滿、沒有 Boss 引擎的早期地圖弓角色
```

變成：

```text
有明確 Boss 按鈕的冷系投射物 Deadeye
```

人話版：第一版報告對 Boss 主訴太溫和了。如果 Boss 要打兩分鐘，這就是傷害引擎修復，不只是抗性修復。抗性要補到不慌，但升級路線必須花在能縮短戰鬥的部位：gem level、jewel、rare ring、quiver、bow、Boss supports。
