---
# === Identity ===
slug: "regulatory-lag"
type: "pattern"

# === Definition ===
name: "後追い規制パターン"
formula: "innovation(t) → dominance(t+3) → investigation(t+5) → judgment(t+10)"
description: "技術革新のスピードに規制が構造的に追いつけず、判決が出る頃には企業は次の市場へ移動済み。規制の本質的限界。"

# === Components ===
components:
  - name: "innovation(t)"
    description: "技術革新・新市場の創出"
  - name: "dominance(t+3)"
    description: "市場支配の確立（イノベーション後3-5年）"
  - name: "investigation(t+5)"
    description: "規制当局の調査開始（支配確立後2-3年）"
  - name: "judgment(t+10)"
    description: "判決・和解（調査開始後5年程度）"

# === Instances ===
instances:
  - entity: "microsoft-ie-timeline"
    layer: "technology"
    note: "1995年IE登場 → 1998年提訴 → 2001年和解（6年）"
  - entity: "google-shopping-timeline"
    layer: "technology"
    note: "2004年Shopping開始 → 2010年調査 → 2017年判決（13年）"
  - entity: "facebook-cambridge-timeline"
    layer: "technology"
    note: "2014年データ取得 → 2018年発覚 → 2019年和解（5年）"

# === Labels ===
labels: ["regulatory-failure", "time-lag", "structural-disadvantage"]

# === Meta ===
updated: 2026-02-25
---

# 後追い規制パターン

## 構造式

```
innovation(t) → dominance(t+3) → investigation(t+5) → judgment(t+10)
      ↓              ↓                 ↓                  ↓
  技術革新       市場支配確立        調査開始           判決
  (新市場)      (3-5年後)         (5-8年後)        (10-15年後)
                                                        ↓
                                              企業は次の市場へ移動済み
```

## 核心

規制は構造的に「後追い」になる。
判決が出る頃には、その市場は成熟し、企業は次の市場で同じパターンを繰り返している。

## メカニズム

### タイムラインの構造

```
Year 0  : 技術革新（新サービス開始）
Year 1-3: 急成長（規制当局は「様子見」）
Year 3-5: 市場支配確立（競合排除完了）
Year 5-7: 問題の顕在化（被害者の声）
Year 7-9: 調査開始（証拠収集）
Year 9-12: 法的手続き（裁判/交渉）
Year 12-15: 判決/和解
Year 15+: 次の市場で同じことが進行中
```

### なぜ追いつけないか

| 要因 | 規制側 | 企業側 |
|------|--------|--------|
| スピード | 行政手続き（年単位） | 製品サイクル（月単位） |
| 専門知識 | 一般法律家 | 特化エンジニア |
| リソース | 公的予算 | 無制限の法務費用 |
| インセンティブ | 「失敗を避ける」 | 「勝つ」 |

## 適用例

### テクノロジー（タイムライン）

| Entity | Innovation | Dominance | Investigation | Judgment | Lag |
|--------|------------|-----------|---------------|----------|-----|
| Microsoft IE | 1995 | 1998 | 1998 | 2001 | 6年 |
| Google Shopping | 2004 | 2008 | 2010 | 2017 | 13年 |
| Google Android | 2008 | 2012 | 2015 | 2018 | 10年 |
| Facebook Privacy | 2014 | 2016 | 2018 | 2019 | 5年 |
| Microsoft Azure | 2010 | 2020 | 2026 | ? | 16年+ |

### パターンの予測

| Entity | Current Market | Next Market | Predicted Investigation |
|--------|---------------|-------------|------------------------|
| Microsoft | Azure (2026調査中) | AI/Copilot | 2030-2032 |
| Google | 広告 (2019判決済) | AI/Gemini | 2028-2030 |
| Amazon | EC (2022和解済) | AI/Alexa | 2027-2029 |

## 構造が維持される理由

1. **事後規制の限界**: 違反後に対応する仕組み
2. **事前規制のジレンマ**: イノベーション阻害の批判
3. **複雑性の非対称**: 企業は自社システムを理解、規制は外から推測
4. **リボルビングドア**: 規制当局と企業の人材交流

## 破壊条件

- **事前規制の導入**（EUのDMA: 指定企業への事前義務）
- **リアルタイム監視**（アルゴリズム監査の義務化）
- **構造的分離**（金融規制のような業務分離）

## 関連パターン

- [[platform-adjacency]] - 隣接市場への触手パターン
- [[penalty-as-license]] - 制裁金＝営業許可料パターン

## 哲学的接続

- **ゼノン**: アキレスは亀に追いつけない → 規制は企業に追いつけない
- **ヘーゲル**: 「ミネルヴァの梟は黄昏に飛び立つ」→ 哲学/規制は事後的
- **マルクス**: 上部構造（法）は下部構造（経済）に遅れて追随する
