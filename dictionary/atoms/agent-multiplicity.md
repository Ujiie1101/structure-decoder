---
id: "agent-multiplicity"
name: "行為者多重性"
type: "atom"
domain: "social"
created: 2026-04-29
---

# 行為者多重性

介入後の系に存在する**多数の独立した行為者**。各々が介入に応じて行動を変えるため、結果が単一行為者の意思から大きく逸脱する。

## 起源（Why this exists）

社会・経済・政治のシステムには、常に多数の独立した意思決定主体が存在する。政策が施行されれば、企業・市民・関連組織がそれぞれ反応する。それぞれの反応が他者の反応を変える。**反応の連鎖**は、初期介入者が想定した範囲を必ず超える。

これは「行為者が悪意を持つ」のではない。各行為者は**自分の合理性**で動く。だが多数の合理が衝突・補完・打ち消し合うと、結果は誰も意図しなかった形になる。

これは部分の和が全体にならない、という創発の原理に基づく構造。

## 観察可能なproxy

- 政策介入後の各セクター（業界・住民・周辺国）の反応速度
- 介入時点で想定された行為者数 vs 実際に反応した行為者数
- 「予想外の反応」を示した行為者の数
- ゲーム理論的均衡分析の事前実施有無

## 介入点（Disable conditions）

- 多主体シミュレーションの事前実施（agent-based modeling）
- 介入対象の絞り込み（影響受ける行為者数を限定）
- 段階的施行（パイロット → 本格展開）
- 行為者ごとのインセンティブ設計

## 関与パターン

- [unintended-consequences](../patterns/unintended-consequences.md) — 結果の分散源
- （拡張候補: cascade, network-effect, prisoners-dilemma）

## 補足

このatomは [causal-distance] × [second-order-blindness] と組み合わさって unintended-consequences を生む。

- causal-distance: 結果が顕在化する**遠さ**
- second-order-blindness: 結果を予測する**能力不足**
- agent-multiplicity: 結果を**分散させる**多主体性

3つが揃ったとき、合理的介入が予期せぬ結果を生む。介入そのものを止めるのではなく、3つそれぞれへの対策が必要。
