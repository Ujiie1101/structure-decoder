---
id: "warning"
name: "警告"
grammar_type: "emergence"
mechanism_id: "E-151"
created: 2026-03-11
---

# warning（警告）

危険や問題を事前に知らせ、予防的行動を促す情報伝達の構造。

## 定義

潜在的リスク・異常・脅威を検知し、関係者に伝達することで、損害を回避または軽減するための予防的行動を可能にする。

## 構造

```
risk_detection
  → signal_interpretation
    → information_transmission
      → recipient_awareness
        → preventive_action (damage averted or mitigated)
```

## 発動条件

1. リスク検知メカニズムの存在
2. シグナルとノイズの識別能力
3. 信頼できる伝達経路
4. 受信者の対応能力

## 失敗条件

- **無視**: 警告の重要性が認識されない
- **過負荷**: 警告過多による鈍感化（狼少年効果）
- **遅延**: 警告が行動可能時間内に届かない
- **曖昧**: 警告内容が不明確で対応できない

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | early-warning-system, cybersecurity-alert, error-message |
| economics | market-indicator, recession-signal |
| history | cassandra-prophecy, intelligence-failure |
| philosophy | precautionary-principle |

## 関連パターン

- **feedback**: 警告は負のフィードバック
- **cascade**: 警告失敗が連鎖的被害を招く
- **fragility**: 警告システムの脆弱性

## メカニズムID

**[E-01] Invisible Hand Coordination** — 分散的警告シグナルから集合的リスク認識が創発
