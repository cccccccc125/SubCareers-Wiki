# 🧑‍⚖️ 權限

> [🏠 首頁](../README.md) · [🔌 安裝](../install.md) · [💾 指令](commands.md) · **🧑‍⚖️ 權限** · [🏷️ 佔位符](placeholders.md) · [🗒️ 設定](config.md)
>
> **副職業**：[⛏️ 採礦](../professions/mining.md) · [🪓 伐木](../professions/logging.md) · [🌾 耕作](../professions/farming.md) · [🎣 釣魚](../professions/fishing.md) · [🌿 草藥](../professions/herb.md) · [⚗️ 煉金](../professions/alchemy.md) · [🔨 鍛造](../professions/forging.md) · [✨ 刻印](../professions/enchanting.md)
>
> **系統**：[🏝️ 空島](../systems/island.md) · [📊 圖鑑](../systems/collections.md) · [🗄️ 資料庫](../systems/database.md) · [🪵 品質素材](../systems/quality-materials.md) · [⭐ 強化](../systems/enhancement.md) · [🪨 礦物融合](../systems/ore-fusion.md)

## 管理權限

| 權限節點 | 預設 | 說明 |
|---------|------|------|
| `subcareers.admin` | OP | 主管理權限 — reload、exp、採礦節點、刻印管理、鍛造管理、強化消耗品 |
| `alchemy.admin` | OP | 煉金系統管理 — wand、create、delete、learn、forget、unlocktier |
| `herb.admin` | OP | 草藥系統管理 — reload |

## 指令權限對照

| 指令 | 所需權限 |
|------|---------|
| `/subcareers reload` | `subcareers.admin` |
| `/subcareers exp add` | `subcareers.admin` |
| `/subcareers exp set` | `subcareers.admin` |
| `/subcareers mining setnode` | `subcareers.admin` |
| `/subcareers mining delnode` | `subcareers.admin` |
| `/subcareers mining list` | `subcareers.admin` |
| `/subcareers enchant give` | `subcareers.admin` |
| `/subcareers forging *` | `subcareers.admin` |
| `/forge bind` | `subcareers.admin` |
| `/forge unbind` | `subcareers.admin` |
| `/forge reload` | `subcareers.admin` |
| `/alchemy wand` | `alchemy.admin` |
| `/alchemy create` | `alchemy.admin` |
| `/alchemy delete` | `alchemy.admin` |
| `/alchemy learn` | `alchemy.admin` |
| `/alchemy forget` | `alchemy.admin` |
| `/alchemy unlocktier` | `alchemy.admin` |
| `/alchemy reload` | `alchemy.admin` |
| `/subcareers herb reload` | `herb.admin` |
| `/island delete` | `subcareers.admin` |
| `/subcareers givescroll` | `subcareers.admin` |

## 玩家指令（無需權限）

`/subcareers`、`/subcareers help`、`/subcareers enchant list`、`/subcareers enhance`、`/subcareers starupgrade`、`/subcareers fusion`、`/fusion`、`/rodeditor`、`/fishbag`、`/island`、`/island leave`、`/island tpset`、`/island visit`、`/island invite`、`/island uninvite`、`/island kick`、`/forge help`、`/alchemy help`
