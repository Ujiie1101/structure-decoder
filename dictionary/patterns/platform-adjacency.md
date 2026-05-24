---
# === Identity ===
slug: "platform-adjacency"
type: "pattern"

# === Definition ===
name: "隣接市場への触手パターン"
formula: "dominance(A) → expansion(B) → regulation(lag) → escape(C)"
description: "支配的地位を持つ市場Aから隣接市場Bへ強制誘導し独占を確立。規制が追いつく頃には次の市場Cへ移動済み。プラットフォーム経済の根本構造。"

# === Components ===
components:
  - name: "dominance(A)"
    description: "既存市場での支配的地位"
  - name: "expansion(B)"
    description: "隣接市場への強制誘導（バンドリング、差別的価格など）"
  - name: "regulation(lag)"
    description: "規制当局の後追い対応"
  - name: "escape(C)"
    description: "次の市場への移動（規制完了時には確立済み）"

# === Instances ===
instances:
  - entity: "microsoft-ie-1998"
    layer: "technology"
    note: "Windows支配 → ブラウザ強制 → 行動規制 → 次はMedia Player"
  - entity: "microsoft-azure-2026"
    layer: "technology"
    note: "Office支配 → Azure強制 → 立入検査中 → AI市場へ"
  - entity: "google-eu-2017-19"
    layer: "technology"
    note: "検索支配 → Shopping/Android/広告優遇 → 82億ユーロ → AI市場へ"
  - entity: "amazon-ec-2022"
    layer: "technology"
    note: "EC支配 → 自社製品優遇 → 行動規制 → クラウド/AI市場へ"

# === Labels ===
labels: ["platform-power", "regulatory-lag", "market-expansion", "lock-in"]

# === Meta ===
updated: 2026-02-25
---

# 隣接市場への触手パターン

## 構造式

```
dominance(A) → expansion(B) → regulation(lag) → escape(C)
     ↓              ↓              ↓               ↓
  既存支配      強制誘導       後追い規制      次の市場へ
  (OS, 検索)   (バンドリング)   (3-10年遅れ)    (規制前に確立)
```

## 核心

プラットフォームは「支配的地位」を「てこ」にして隣接市場を獲得する。
規制当局は構造的に後追いになり、追いつく頃には次の戦場へ移動済み。

## メカニズム

### 1. 強制誘導の手段

| 手段 | 例 |
|------|-----|
| バンドリング | Windows + IE、Office + Teams |
| 差別的価格 | Azure以外でのライセンス料引き上げ |
| 技術的ロックイン | 「他社製品では不具合が生じる」 |
| データ優位の流用 | EC出品者データを自社製品開発に利用 |

### 2. 規制ラグのタイムライン

```
Year 0   : イノベーション発生
Year 3-5 : 市場支配確立
Year 5-8 : 規制調査開始
Year 8-13: 判決/和解
Year 13+ : 企業は次の市場で同じことを繰り返し中
```

## 適用例

### テクノロジー

| Year | Entity | Market A | Market B | Market C | Regulation |
|------|--------|----------|----------|----------|------------|
| 1998 | Microsoft | Windows | ブラウザ | Media Player | 行動規制 |
| 2017 | Google | 検索 | Shopping | 広告 | 24億ユーロ |
| 2018 | Google | 検索 | Android | AI | 43億ユーロ |
| 2022 | Amazon | EC | 自社製品 | クラウド | 行動規制 |
| 2026 | Microsoft | Office | Azure | AI | 進行中 |

### 歴史的先例

| Era | Entity | Market A | Market B | Regulation |
|-----|--------|----------|----------|------------|
| 1900s | Standard Oil | 精製 | 流通 | 分割（唯一の成功例）|
| 1980s | AT&T | 長距離通信 | 機器 | 分割 |

## 構造が維持される理由

1. **ネットワーク効果**: 勝者総取りの市場構造
2. **分割の政治的困難**: 地政学的理由で保護
3. **代替の不在**: 規制しても乗り換え先がない

## 破壊条件

- **分割命令**（歴史的に稀、AT&T/Standard Oilのみ）
- **相互運用性義務**（EUのDMAが実験中）
- **技術的破壊**（分散型システムによる中央集権の無効化）

## 関連パターン

- [[hubris-nemesis]] - 傲慢パターン（成功の内部化）
- [[regulatory-lag]] - 後追い規制パターン
- [[penalty-as-license]] - 制裁金＝営業許可料パターン

## 哲学的接続

- **マルクス**: 「歴史は繰り返す、一度目は悲劇として、二度目は茶番として」
- **フーコー**: 権力は遍在し、抑圧するのではなく生産する
- **ヘラクレイトス**: 表面は変わる（IE→Azure→AI）、構造は同じ（隣接市場への拡張）
