# 🪨 礦物融合

> [🏠 首頁](../README.md) · [🔌 安裝](../install.md) · [💾 指令](../general/commands.md) · [🧑‍⚖️ 權限](../general/permissions.md) · [🏷️ 佔位符](../general/placeholders.md) · [🗒️ 設定](../general/config.md)
>
> **副職業**：[⛏️ 採礦](../professions/mining.md) · [🪓 伐木](../professions/logging.md) · [🌾 耕作](../professions/farming.md) · [🎣 釣魚](../professions/fishing.md) · [🌿 草藥](../professions/herb.md) · [⚗️ 煉金](../professions/alchemy.md) · [🔨 鍛造](../professions/forging.md) · [✨ 刻印](../professions/enchanting.md)
>
> **系統**：[🏝️ 空島](island.md) · [📊 圖鑑](collections.md) · [🗄️ 資料庫](database.md) · [🪵 品質素材](quality-materials.md) · [⭐ 強化](enhancement.md) · **🪨 礦物融合**

## 概述

礦物融合系統允許玩家依設定配方，將多個礦物素材合成為更高級的材料。

## 開啟方式

- `/fusion` — 開啟礦物融合介面（快捷指令）
- `/subcareers fusion` — 同上

## 介面說明

### 配方列表（54 格）

顯示所有可用的融合配方。每個圖示格顯示：
- 所需輸入材料與數量
- 合成後輸出材料

點擊任意配方後進入確認介面。

### 確認介面（27 格）

顯示所選配方的詳細資訊。確認後系統自動從背包扣除所需材料，並將輸出材料放入背包。

## 設定檔 (`mining/mining.yml`)

```yaml
ore-fusion:
  IRON_INGOT_MEDIUM:
    input: "MATERIAL/IRON_ORE"
    input-amount: 3
    output: "MATERIAL/IRON_INGOT_MEDIUM"
    output-amount: 1
  GOLD_INGOT_MEDIUM:
    input: "MATERIAL/GOLD_ORE"
    input-amount: 3
    output: "MATERIAL/GOLD_INGOT_MEDIUM"
    output-amount: 1
  DIAMOND_MEDIUM:
    input: "MATERIAL/DIAMOND_ORE"
    input-amount: 3
    output: "MATERIAL/DIAMOND_MEDIUM"
    output-amount: 1
```

| 欄位 | 說明 |
|------|------|
| `input` | 輸入材料（`MATERIAL/<MMOItems ID>` 格式） |
| `input-amount` | 需要的數量 |
| `output` | 輸出材料（`MATERIAL/<MMOItems ID>` 格式） |
| `output-amount` | 輸出數量 |

配方 ID（最外層 key）僅作識別用，顯示名稱從 MMOItems 物品定義讀取。
