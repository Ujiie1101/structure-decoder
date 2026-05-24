---
# === Identity ===
slug: "penalty-as-license"
type: "pattern"

# === Definition ===
name: "制裁金＝営業許可料パターン"
formula: "violation → penalty → cost-absorption → continuation"
description: "制裁金が「罰」ではなく「事業コスト」として織り込まれ、違反行為の継続を許可する構造。抑止力の無効化。"

# === Components ===
components:
  - name: "violation"
    description: "法令違反・独占的行為"
  - name: "penalty"
    description: "制裁金・罰金"
  - name: "cost-absorption"
    description: "事業コストとして吸収（売上比2-5%程度）"
  - name: "continuation"
    description: "行為の継続（構造は温存）"

# === Instances ===
instances:
  - entity: "google-eu-fines"
    layer: "technology"
    note: "82億ユーロの制裁金、同期間売上4500億ドル超（約2%）"
  - entity: "microsoft-eu-2004"
    layer: "technology"
    note: "20億ユーロ、市場支配は継続"
  - entity: "facebook-ftc-2019"
    layer: "technology"
    note: "50億ドル罰金、株価は上昇（市場は「安い」と判断）"

# === Labels ===
labels: ["regulatory-failure", "cost-of-doing-business", "deterrence-failure"]

# === Meta ===
updated: 2026-02-25
---

# 制裁金＝営業許可料パターン

## 構造式

```
violation → penalty → cost-absorption → continuation
    ↓          ↓            ↓               ↓
  違反      制裁金      コスト化        行為継続
 (独占)    (数十億€)   (売上の2%)    (構造は温存)
```

## 核心

制裁金が抑止力として機能せず、「悪いことを続ける許可料」に転化する。
分割されない限り、支配的地位と構造は温存される。

## メカニズム

### 制裁金 vs 売上の構造

| Entity | Period | Fines | Revenue | Ratio |
|--------|--------|-------|---------|-------|
| Google | 2017-19 | 82億€ | 4500億$+ | ~2% |
| Microsoft | 2004-13 | 20億€ | 3000億$+ | <1% |
| Facebook | 2019 | 50億$ | 700億$ | ~7% |

### なぜ抑止力が効かないか

1. **事前織り込み**: 法務コストとして予算化済み
2. **投資家の反応**: 「不確実性の解消」で株価上昇
3. **行為の継続**: 制裁金を払っても市場支配は維持
4. **分割なし**: 構造的優位は温存

## 適用例

### テクノロジー

| Year | Entity | Violation | Penalty | Outcome |
|------|--------|-----------|---------|---------|
| 2004 | Microsoft | Media Player抱き合わせ | 20億€ | 市場支配継続 |
| 2017 | Google | Shopping優遇 | 24億€ | 同様の行為継続 |
| 2018 | Google | Android抱き合わせ | 43億€ | Android支配継続 |
| 2019 | Facebook | プライバシー侵害 | 50億$ | 株価上昇 |

### 歴史的対比：分割が機能した例

| Year | Entity | Violation | Penalty | Outcome |
|------|--------|-----------|---------|---------|
| 1911 | Standard Oil | 市場独占 | **分割** | 構造的解体 |
| 1984 | AT&T | 市場独占 | **分割** | 競争回復 |

## 構造が維持される理由

1. **地政学的保護**: 自国企業の弱体化は国益に反する
2. **ロビイング**: 政治献金と規制当局への影響力
3. **複雑性**: 市場構造の理解が困難
4. **代替不在**: 規制しても乗り換え先がない

## 破壊条件

- **分割命令**（政治的意志が必要）
- **累積的罰則**（売上の一定%ではなく累積増加）
- **行為差止**（金銭ではなく行為そのものの禁止）

## 関連パターン

- [[platform-adjacency]] - 隣接市場への触手パターン
- [[regulatory-lag]] - 後追い規制パターン
- [[hubris-nemesis]] - 傲慢パターン（「コストで済む」という傲慢）

## 哲学的接続

- **マキャベリ**: 「人は忘れやすい。罰は一度に与えよ」→ 小さな罰の繰り返しは無効
- **ニーチェ**: 「刑罰は犯罪を正当化する」→ 払えば許される構造
- **フーコー**: 「規律権力」から「生権力」へ → 罰ではなく管理
