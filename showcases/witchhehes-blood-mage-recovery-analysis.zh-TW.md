# WitchHehes 血法回血機制分析

來源：公開 poe.ninja 角色頁面  
角色：`WitchHehes`，91 級 Blood Mage，Runes of Aldur  
URL: https://poe.ninja/poe2/builds/runesofaldur/character/Urbanspaghett-3756/WitchHehes?i=17&search=class%3DBlood%2BMage%26sort%3Ddps

## 簡短結論

這個 build 不是主要靠傳統吸血回血。

它的回復結構是一個分層的 Blood Mage / Archmage 生存系統：

1. `Life Remnants` 回血。
2. `Mana Remnants` 回魔。
3. `Mind Over Matter` 讓 Mana 先替 Life 吃傷害。
4. `Eldritch Battery` 把 Energy Shield 轉成最大 Mana。
5. `Vitality II`、擊殺回血、藥水、護符提供小額兜底。

所以答案是：

> 它不是靠裝備上一條明顯的 leech 活著，而是靠 Remnant 循環回血/回魔，並用大 Mana 池擋在 Life 前面。

## 觀察到的防禦面板

poe.ninja 當時資料：

- Life: `2682`
- Mana: `3858`
- Energy Shield: `0`
- Life Regeneration: `53/sec`
- Effective Health Pool: `15542`
- Physical Max Hit: `7447`
- Fire Max Hit: `26550`
- Cold Max Hit: `17288`
- Lightning Max Hit: `26550`
- Chaos Max Hit: `20650`

重點是資源結構：血不高，魔很高，ES 為 0。

這和它點的兩個關鍵機制對上：

- `Mind Over Matter`: 所有傷害先從 Mana 扣，再扣 Life，但 Mana Recovery Rate 降低。
- `Eldritch Battery`: 把最大 Energy Shield 轉成最大 Mana。

所以這裡的 Mana 不是普通施法資源，而是第一層防禦血條。

## 主回血：Life Remnants

技能連結：

```text
Life Remnants L20
Harmonic Remnants II
Remnant Potency III
```

`Life Remnants` 觀察到的效果：

- Remnants 持續 8 秒。
- 擊殺敵人有 25% 機率生成 Remnant。
- 命中目標時生成 Remnant，每 3 秒最多一次。
- 每個 Remnant 給 `410 Life`。

`Remnant Potency III` 提供：

- Supported Skill 生成的 Remnant 效果提高 40%。
- 收集後延遲 3 秒生效。

粗算一個 Life Remnant：

```text
410 * 1.4 = 574 Life
```

這才是它真正的 Life 回復引擎，只是不會像裝備 leech 那樣一眼看出來。

## 主防禦回復：Mana Remnants

技能連結：

```text
Mana Remnants L19
Harmonic Remnants II
Remnant Potency III
```

`Mana Remnants` 觀察到的效果：

- Remnants 持續 8 秒。
- 擊殺帶元素異常的敵人時有 25% 機率生成 Remnant。
- 暴擊命中帶元素異常的目標時生成 Remnant，每 2 秒最多一次。
- 每個 Remnant 給 `311 Mana`。

配合 `Remnant Potency III`，粗算：

```text
311 * 1.4 = 435 Mana
```

因為 `Mind Over Matter` 會讓 Mana 先承傷，所以 Mana Remnants 實際上也是防禦回復。

這就是這個 build 難看懂的地方：它把回復拆成兩條線，一條補 Life，一條補 Mana 護城河。

## 次要回復來源

這些也存在，但不是核心：

### `Malice + Vitality II`

`Vitality II` 提供：

```text
Supported persistent buff active 時，每秒回復 2% maximum Life
```

以 `2682 Life` 計算：

```text
2682 * 0.02 = 53.6 Life/sec
```

poe.ninja 面板顯示 `53/sec`，完全對上。

### 戒指擊殺回血

一個戒指有：

```text
Gain 50 Life per enemy killed
```

對刷圖有幫助，但不要當成 boss 戰主要回復。

### 藥水和護符

觀察到的藥水/護符回復：

- Life Flask: `920 Life over 3 seconds`
- Life Flask: `29% of recovery applied instantly`
- 腰帶 implicit: `20% of flask recovery applied instantly`
- 護符：被暈時回復 `345 Life`

這些是緊急兜底或刷圖輔助，不是主循環。

## 為什麼容易看漏

如果只找這些關鍵詞，很可能找不到答案：

- Life leech
- Damage leeched as Life
- 大量 regen
- instant Life on hit

真正的答案藏在技能和 keystone 組合裡：

```text
Life Remnants + Mana Remnants + Mind Over Matter + Eldritch Battery
```

它同時維護兩個池子：

- Life 靠 Life Remnants 補。
- Mana 靠 Mana Remnants 補，而 Mana 因為 MoM 先吃傷害，所以等於 Life 前面的第二血條。

## 抄作業注意點

如果要抄這個 build，不能只抄傷害技能。

回復包需要一起抄：

1. `Life Remnants`，並用 support 提高球的價值。
2. `Mana Remnants`，用來維持 Mana 防禦池。
3. 足夠暴擊/元素異常，穩定觸發 Mana Remnants。
4. 足夠最大 Mana，讓 `Mind Over Matter` 真有意義。
5. 操作上要能舒服吃球，因為 Remnants 需要撿。

如果這些缺了，角色可能看起來 DPS 很高，但實際會很脆。

