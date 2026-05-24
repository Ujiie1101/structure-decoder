---
id: "invention-failure"
name: "発明失敗"
grammar_type: "emergence"
mechanism_id: "E-075"
created: 2026-03-11
---

# invention-failure（発明失敗）

技術的成功にもかかわらず、市場・社会・タイミングの不適合により価値実現に失敗する構造。

## 定義

発明それ自体は技術的に成功しているが、市場ニーズ・社会受容・ビジネスモデル・タイミングとの不整合により、商業的・社会的価値を生み出せない。成功した発明が失敗する逆説的パターン。

## 構造

```
technical_success
  → market_misalignment
    → adoption_failure
      → resource_exhaustion
        → value_unrealized (despite innovation)
```

## 発動条件

1. 技術と市場ニーズの乖離
2. 過早（too early）または過遅（too late）
3. 補完的資産の不足
4. ビジネスモデルの欠如

## 失敗条件

- **技術的優位性の過信**: 技術が優れていれば売れるという錯覚
- **市場調査の欠如**: 顧客ニーズの誤認
- **エコシステム無視**: インフラ・補完財の不在
- **資金枯渇**: 市場成熟前の撤退

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | xerox-parc, webvan, segway, google-glass, newton |
| economics | concorde, betamax |
| history | tesla-ac-invention, da-vinci-inventions |
| science | cold-fusion |

## 関連パターン

- **emergence**: 市場・技術の整合から価値が創発
- **disruption**: 成功した破壊的イノベーションとの対比
- **substitution**: 後発の代替技術による置換

## メカニズムID

**[E-05] Innovation-Market Mismatch** — 技術と市場の不整合から価値未実現が生じる
