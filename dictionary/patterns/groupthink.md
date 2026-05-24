---
id: "groupthink"
name: "集団思考"
grammar_type: "emergence"
mechanism_id: "E-060"
created: 2026-03-11
composition:
  - atom: conformity-pressure
    role: 自分から多数派に同期する内圧
  - atom: dissent-suppression
    role: 異論者を罰する集団内の外圧
  - atom: illusion-of-unanimity
    role: 沈黙を同意と誤読する集合的錯覚
composition_formula: "conformity-pressure × dissent-suppression × illusion-of-unanimity"
composition_note: "三atomは独立だが循環する: 過去の dissent-suppression の記憶が conformity-pressure を生み、結果として全員が黙り、illusion-of-unanimity が成立する。介入はループのどこかで切る必要がある。"
---

# groupthink（集団思考）

集団の調和・合意を優先するあまり、批判的思考や異論が抑制される構造。

## 定義

凝集性の高い集団において、合意形成への圧力が個人の批判的評価能力を抑制し、非合理的・機能不全な意思決定が行われる現象。

## 構造

```
cohesive_group
  → consensus_pressure
    → self_censorship
      → illusion_of_unanimity
        → defective_decision (critical thinking suppressed)
```

## 発動条件

1. 高い集団凝集性
2. 外部からの隔離
3. 強力なリーダーシップ
4. 代替案検討手続きの不在

## 失敗条件

- **多様性**: 異なる視点の制度的確保
- **悪魔の代弁者**: 批判役の明示的設定
- **外部評価**: 第三者による検証
- **匿名性**: 意見表明の心理的安全性

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | echo-chamber, filter-bubble |
| economics | market-bubble, herd-behavior |
| history | bay-of-pigs, challenger-disaster |
| philosophy | mob-mentality, conformity |

## 関連パターン

- **cascade**: 集団思考による誤りの連鎖
- **feedback**: 合意圧力の自己強化
- **coordination-failure**: 集団思考による調整失敗

## メカニズムID

**[E-01] Invisible Hand Coordination** — 個々の自己検閲から集合的盲点が創発
