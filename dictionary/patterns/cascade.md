---
id: "cascade"
name: "連鎖"
grammar_type: "cascade"
mechanism_id: "A-001"
created: 2026-03-11
composition:
  - atom: interconnection-density
    role: 連鎖の物理的前提となるネットワーク構造
  - atom: state-coupling
    role: ノード間で状態が機械的に伝播する駆動力
  - atom: damping-absence
    role: 連鎖を止める制動機構の不在
composition_formula: "interconnection-density × state-coupling × damping-absence"
composition_note: "接続が密でも結合が弱ければ連鎖しない。結合があっても減衰機構があれば局所化する。三者揃って初めて全面的連鎖が成立する。"
---

# cascade（連鎖）

一つの出来事が次々と他の出来事を誘発する構造。

## 定義

初期イベントが、相互接続されたシステム内で連鎖反応を引き起こし、影響が指数関数的に拡大する。ドミノ効果、感染、バイラル拡散などを含む。

## 構造

```
initial_event
  → primary_effects
    → secondary_effects (amplified)
      → tertiary_effects (further amplified)
        → systemic_impact
```

## 発動条件

1. 相互接続性（ネットワーク構造）
2. 増幅メカニズム（正のフィードバック）
3. 閾値を超えるトリガー
4. 伝播経路の存在

## 失敗条件（連鎖停止）

- **分断**: ネットワークの断絶
- **減衰**: 伝播力の弱さ
- **介入**: 人為的遮断
- **飽和**: 影響可能な対象の枯渇

## 適用事例

| Layer | Entities |
|-------|----------|
| economics | financial-contagion, bank-run |
| politics | revolution-spread, domino-theory |
| technology | viral-spread, network-effects |
| history | arab-spring, 1848-revolutions |
| art | trend-diffusion |

## 関連パターン

- **collapse**: 連鎖的崩壊
- **emergence**: 連鎖からの創発
- **amplification**: 連鎖の増幅

## メカニズムID

**[C-02] Confidence Contagion** — 信頼/不信の伝染
**[MP-01] Reflexive Spiral** — 反射的スパイラル
