---
id: "prevention"
name: "予防"
grammar_type: "emergence"
layer: 3
mechanism_id: "E-106"
domains: ["technology"]
created: 2026-03-11
---

# prevention（予防）

問題が発生する前に対策を講じることで、損害を未然に防ぐ構造。

## 定義

リスクや問題の発生を事前に予測し、先制的な介入によって被害を回避または最小化する。治療より予防のコストが低いという経済論理と、不確実性下での意思決定という哲学的問題を含む。

## 構造

```
risk_identification
  → probability_assessment
    → preemptive_intervention
      → harm_avoidance
        → feedback_to_risk_model
```

## 発動条件

1. リスクの識別・予測可能性
2. 介入手段の存在
3. 予防コスト < 期待損害
4. 介入のタイミング確保

## 失敗条件

- **過剰予防**: コストが便益を上回る
- **予測失敗**: リスク評価の誤り
- **偽陽性**: 不要な介入による弊害
- **予防のパラドックス**: 成功が予防の必要性を見えなくする

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | antivirus, firewall, predictive-maintenance |
| economics | hedging, insurance, reserve-requirement |
| philosophy | precautionary-principle, risk-ethics |
| history | vaccination, public-health |
| society | crime-prevention, disaster-preparedness |

## 関連パターン

- **emergence**: 予防システムからの新秩序創発
- **feedback**: 予防結果のフィードバック
- **constraint**: 予防的制約
