---
id: "non-iteration"
name: "非反復性"
type: "atom"
domain: "social"
created: 2026-04-29
---

# 非反復性

同じ相手との将来の取引が**期待できない**状態。一回限りのゲームの構造的特性。

## 起源（Why this exists）

反復ゲームでは、今日の裏切りが明日の報復を招く。将来の損失予期が、現在の協力選択を支える。Robert Axelrod の "tit-for-tat" 戦略の有効性は、反復の存在に依存する。

非反復状態では、この機構が作動しない。今日の裏切りは今日のゲームで完結し、明日の罰は存在しない。結果として協力選択の合理的根拠が消える。

非反復性は様々な状況で発生する：
- 一期一会の取引（観光地、転売）
- 終末期（引退間際の経営者、選挙最後の議員）
- 高速変化（短期間で相手が変わる業界）
- 大規模匿名（誰と取引したか追跡できない）

## 観察可能なproxy

- 取引の継続予測（何回続くか）
- 相手の特定可能性（同じ相手と再取引できるか）
- 業界・市場の変化速度
- 人間関係の流動性（転職率、引っ越し率）
- 「最後の取引」が予期される文脈

## 介入点（Disable conditions）

- 反復化（短期取引を長期契約に変換）
- 評判の集約（個別の非反復取引を、評判という反復装置に集約）— ECサイトの星評価
- 長期コミュニティ化（取引相手を固定）
- 引退・終末の延期や曖昧化

## 関与パターン

- [prisoners-dilemma](../patterns/prisoners-dilemma.md) — 報復不能による脱出阻害
- （拡張候補: end-game-problem, last-period-defection, drive-by-economics）

## 補足

[commitment-impossibility] との違い:
- **commitment-impossibility**: 将来の自分の行動を約束する装置がない
- **non-iteration**: 将来の相手との取引そのものがない

前者は「約束しても破れる」、後者は「そもそも将来の出会いがない」。前者は時間内構造の問題、後者は時間軸そのものの欠如。

prisoners-dilemma の三atom（dominant-defection × commitment-impossibility × non-iteration）はそれぞれ独立した条件。利得構造（経済）×制度（institutional）×時間（social）の三軸で構成される。
