---
id: "dilemma"
name: "ジレンマ"
grammar_type: "emergence"
mechanism_id: "E-038"
created: 2026-03-11
---

# dilemma（ジレンマ）

相互に排他的な選択肢の間で、どちらを選んでも損失が生じる構造。

## 定義

二つ以上の選択肢が存在するが、各選択肢は他の重要な価値を犠牲にする。完全な解決策が存在せず、トレードオフの最適化が問われる。構造的制約から生じる必然的緊張状態。

## 構造

```
competing_values (A vs B)
  → mutual_exclusivity
    → forced_choice
      → inevitable_loss (one or both sides)
        → tension_persists (no perfect solution)
```

## 発動条件

1. 複数の正当な価値・目標の存在
2. 資源・時間・論理的制約
3. 選択の不可避性
4. トレードオフ構造

## 失敗条件

- **偽りの二項対立**: 第三の選択肢の見落とし
- **時間軸の無視**: 短期 vs 長期の調停可能性
- **部分最適化**: 全体最適の欠如
- **フレーミング固定**: 問題設定自体の変更可能性

## 適用事例

| Layer | Entities |
|-------|----------|
| philosophy | trolley-problem, liberty-equality |
| economics | inflation-unemployment, efficiency-equity |
| technology | privacy-convenience, security-usability, innovators-dilemma |
| history | appeasement-war, intervention-sovereignty |
| religion | faith-reason, tradition-reform |

## 関連パターン

- **emergence**: ジレンマから新しい解決策が創発する可能性
- **equilibrium**: ジレンマの動的均衡点
- **oscillation**: ジレンマの両極間の振動

## メカニズムID

**[E-09] Structural Tension** — 構造的制約から不可避の緊張が生じる
