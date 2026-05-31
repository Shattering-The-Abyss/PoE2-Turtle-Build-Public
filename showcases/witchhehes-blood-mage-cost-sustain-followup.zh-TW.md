# WitchHehes 血法追蹤分析：技能消耗怎麼維持

來源：公開 poe.ninja 角色頁面  
角色：`WitchHehes`，91 級 Blood Mage，Runes of Aldur  
相關報告：[WitchHehes 血法回血機制分析](witchhehes-blood-mage-recovery-analysis.zh-TW.md)

## 簡短結論

這次補上的關鍵層不是「它怎麼回血」。

更精確的問題是：

> 如果 Mana 透過 Mind Over Matter 變成防禦血條，那它怎麼避免技能把 Mana 花光？

答案是：

> 它把大量技能消耗從 Mana 挪到 Life，然後用 Life Remnants 把這個 Life 成本補回來。Mana 盡量保留給防禦，再靠 Mana Remnants、擊殺回魔、魔水補回來。

## 核心資源循環

```text
技能消耗 Life / 部分 Life
Life Remnants 補 Life
Mana 保留下來當 Mind Over Matter 防禦池
Mana Remnants 在受傷或消耗後補 Mana
```

所以它不是簡單的：

```text
Mana = Life
```

更準確是：

```text
Life 負責付技能費。
Mana 負責吃進來的傷害。
Remnants 同時補兩個池子。
```

## 證據：Lifetap 到處都是

這些主動技能都帶了 `Lifetap`：

- `Spark`
- `Lightning Bolt`
- `Orb of Storms`
- `Cast on Critical + Comet`
- `Frost Bomb`
- `Spellslinger + Living Bomb`
- `Elemental Weakness`

這是最大線索。這個 build 不希望普通施法把 Mana 池打空，因為 Mana 同時是防禦池。

## 證據：武器把法術 Mana Cost 轉成 Life Cost

它的 wand 有：

```text
16% of Spell Mana Cost Converted to Life Cost
```

這和 Lifetap 是同一個方向：

```text
降低 Mana 壓力。
把施法成本轉到 Life。
用 Remnants 把 Life 補回來。
```

這點尤其重要，因為它用了 `Eldritch Battery`，而 EB 會讓 Mana Costs doubled。

## 為什麼必須這樣做

它用了：

```text
Mind Over Matter
Eldritch Battery
```

這兩個 keystone 組合很強，但資源結構很彆扭：

- `Mind Over Matter`: 所有傷害先從 Mana 扣，再扣 Life，但 Mana Recovery Rate 降低。
- `Eldritch Battery`: Energy Shield 轉成最大 Mana，但 Mana Costs doubled。

如果它所有法術都用 Mana 支付，就會把自己用來防禦的池子花掉。

所以它用 Life 去承擔大部分施法成本。

## Life 成本怎麼補

Life 側靠：

```text
Life Remnants L20
Harmonic Remnants II
Remnant Potency III
```

觀察到的數值：

```text
每個 Remnant 給 410 Life
Remnant Potency III 提高 40% effect
約等於每個 Life Remnant 給 574 Life
```

所以 `Life Remnants` 同時做兩件事：

1. 補實際打到 Life 的傷害。
2. 補 Lifetap / 法術轉 Life cost 花掉的 Life。

## Mana 防禦池怎麼補

Mana 側靠：

```text
Mana Remnants L19
Harmonic Remnants II
Remnant Potency III
```

觀察到的數值：

```text
每個 Remnant 給 311 Mana
Remnant Potency III 提高 40% effect
約等於每個 Mana Remnant 給 435 Mana
```

它還有一個 unique jewel 詞綴：

```text
Recover 2% of maximum Mana on Kill
```

以 `3858 Mana` 計算，大約是：

```text
每擊殺回 77 Mana
```

它也帶了魔水：

```text
29% of Recovery applied Instantly
48% increased Charges
```

所以刷圖時 Mana 續航大概是：

- Mana Remnants
- 擊殺回復 2% 最大 Mana
- 魔水
- 透過 Lifetap 避免直接花太多 Mana

## 最終判斷

這是一個雙資源維持系統：

```text
Life 側：
Lifetap / 轉換成本 -> Life Remnants 補回來

Mana 側：
Mind Over Matter 防禦池 -> Mana Remnants / 擊殺回魔 / 魔水補回來
```

如果只抄傷害連結，沒抄資源循環，這個 build 很可能會翻車。貴的不只是 DPS，而是 Life 和 Mana 分工明確、各自能補。
