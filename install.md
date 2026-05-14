# 🔌 安裝指南

> [🏠 首頁](README.md) · **🔌 安裝** · [💾 指令](general/commands.md) · [🧑‍⚖️ 權限](general/permissions.md) · [🏷️ 佔位符](general/placeholders.md) · [🗒️ 設定](general/config.md)
>
> **副職業**：[⛏️ 採礦](professions/mining.md) · [🪓 伐木](professions/logging.md) · [🌾 耕作](professions/farming.md) · [🎣 釣魚](professions/fishing.md) · [🌿 草藥](professions/herb.md) · [⚗️ 煉金](professions/alchemy.md) · [🔨 鍛造](professions/forging.md) · [✨ 刻印](professions/enchanting.md)
>
> **系統**：[🏝️ 空島](systems/island.md) · [📊 圖鑑](systems/collections.md) · [🗄️ 資料庫](systems/database.md) · [🪵 品質素材](systems/quality-materials.md) · [⭐ 強化](systems/enhancement.md) · [🪨 礦物融合](systems/ore-fusion.md)

## 環境需求

| 需求 | 版本 | 備註 |
|------|------|------|
| Paper | 1.21.1 | 使用 Spigot API，建議 Paper |
| Java | 21+ | 編譯目標 Java 21 |
| MMOCore | 1.13+ | 必要（softdepend） |
| MMOItems | 6.10+ | 必要（softdepend） |
| MythicLib | 1.7+ | 必要（softdepend） |
| MythicMobs | 5.7.2+ | 可選 — 魚商人 NPC、草藥生怪 |
| Vault | 1.7.4+ | 可選 — 經濟系統（賣魚） |
| SolarTermCore | 1.0+ | 可選 — 節氣加成系統 |
| PlaceholderAPI | 2.x+ | 可選 — 佔位符支援 |

## 安裝步驟

1. 將 `SubCareers.jar` 放入 `plugins/` 資料夾
2. 確保所有相依插件已安裝並正常運作
3. 重啟伺服器
4. 插件會自動在 `plugins/SubCareers/` 產生所有設定檔

## 建議安裝順序

```
1. Vault
2. MythicLib
3. MMOItems
4. MMOCore
5. MythicMobs
6. SolarTermCore
7. SubCareers
```

## 設定 MySQL（選用）

編輯 `plugins/SubCareers/config.yml`：

```yaml
storage-type: mysql

mysql:
  host: localhost
  port: 3306
  database: subcareers
  username: root
  password: your_password
  pool:
    maximum-pool-size: 10
    minimum-idle: 5
    max-lifetime: 1800000
    connection-timeout: 30000
    idle-timeout: 600000
```

若不使用 MySQL，設 `storage-type: yaml`，資料會存在 `plugins/SubCareers/userdata/`。

## 驗證安裝

執行 `/subcareers`，應看到 9 格副職業總覽 GUI。執行 `/subcareers help` 確認所有指令可用。
