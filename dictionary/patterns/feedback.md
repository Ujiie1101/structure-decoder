---
id: "feedback"
name: "フィードバック"
grammar_type: "emergence"
mechanism_id: "E-055"
created: 2026-03-11
---

# feedback（フィードバック）

出力が入力に戻り、システムの挙動を増幅または抑制する構造。

## 定義

システムの結果がシステム自身に影響を与え、その影響がさらなる結果を生む循環構造。正のフィードバックは増幅を、負のフィードバックは安定化をもたらす。

## 構造

```
action
  → output
    → measurement/sensing
      → comparison_to_reference
        → adjustment (reinforcing or dampening)
```

## 発動条件

1. 因果の循環経路
2. 出力の検知メカニズム
3. 入力への影響経路
4. 時間遅延の適切さ

## 失敗条件

- **断絶**: フィードバック経路の切断
- **遅延過大**: 反応が遅すぎて無効化
- **飽和**: 調整能力の限界到達
- **ノイズ**: 信号対雑音比の低下

## 適用事例

| Layer | Entities |
|-------|----------|
| religion | prayer-response, spiritual-discipline, karma |
| economics | price-mechanism, market-correction, inflation |
| technology | thermostat, machine-learning, cybernetics |
| politics | election-cycle, public-opinion |

## 関連パターン

- **amplification**: 正のフィードバック
- **cyclical**: フィードバックが循環を形成
- **emergence**: フィードバックから秩序が創発

## メカニズムID

**[E-01] Invisible Hand Coordination** — フィードバックを通じた自己組織化
