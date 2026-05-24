---
id: "fragility"
name: "脆弱性"
grammar_type: "emergence"
mechanism_id: "E-057"
created: 2026-03-11
---

# fragility（脆弱性）

システムが予測不能なストレスに対して非線形に崩壊する構造。

## 定義

効率性・最適化の追求により余剰・冗長性が排除され、小さなショックに対しても不均衡な損害を被りやすくなった状態。安定が脆弱性を蓄積させる。

## 構造

```
optimization_for_efficiency
  → elimination_of_redundancy
    → hidden_vulnerability_accumulation
      → small_shock_arrives
        → nonlinear_collapse (convex harm)
```

## 脆弱性の特徴

- **非線形性**: 衝撃の2倍が損害の2倍以上
- **凹性（Concavity）**: 利得より損失が大きい
- **隠れた依存性**: 想定外の相関が顕在化
- **尾部リスク**: 分布の端で破滅的損害

## 発動条件

1. 効率化による冗長性の排除
2. システムの相互連結性
3. 大きな変動の過小評価
4. ストレスからの学習機会の欠如

## 対照概念：Antifragility

Nassim Talebが提唱。ストレスから利益を得る性質。

| 脆弱 | 頑健 | 反脆弱 |
|------|------|--------|
| 凹型損害 | 線形反応 | 凸型利得 |
| ボラティリティを嫌う | 中立 | ボラティリティを好む |

## 適用事例

| Layer | Entities |
|-------|----------|
| economics | 2008-financial-crisis, supply-chain, just-in-time |
| technology | centralized-systems, monoculture |
| history | roman-empire, soviet-collapse |
| philosophy | black-swan, uncertainty |

## 関連パターン

- **self-undermining-success**: 成功による最適化が脆弱性を増大
- **cascade**: 脆弱性が連鎖的崩壊を可能にする
- **emergence**: 頑健性は複雑系の創発特性

## 注意

「安定しているから安全」は危険な錯覚。長期安定は小さなストレスを抑圧し、大きな破壊を準備している可能性がある。Great Moderationから2008年金融危機へ。
