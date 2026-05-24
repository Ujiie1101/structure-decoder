---
id: "substitution"
name: "代替"
grammar_type: "substitution"
mechanism_id: "S-001"
created: 2026-03-11
---

# substitution（代替）

既存の制度・技術・概念が、新しいものに置き換えられる構造。

## 定義

ある機能を担っていた既存システムが、同等またはより優れた機能を持つ新システムに取って代わられる。旧システムは縮小・消滅するか、ニッチに追いやられる。

## 構造

```
incumbent_system (function F)
  → challenger_emerges (function F')
    → performance_crossover (F' > F)
      → adoption_cascade
        → incumbent_displacement
          → new_dominant_system
```

## 発動条件

1. 既存システムの機能不全または非効率
2. 代替候補の出現
3. 切り替えコストを上回る便益
4. 採用の臨界量到達

## 失敗条件

- **ロックイン**: 既存システムへの過剰投資
- **ネットワーク効果**: 既存システムの普及率が高すぎる
- **規制障壁**: 法的保護による新規参入阻止
- **不完全代替**: 新システムが旧機能を完全カバーできない

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | digital-photography, streaming |
| economics | cryptocurrency, gig-economy |
| politics | regime-change, constitutional-revision |
| religion | reformation, new-religious-movements |
| art | avant-garde, new-media |

## 関連パターン

- **erosion**: 代替に先立つ既存システムの弱体化
- **collapse**: 代替失敗時の崩壊
- **emergence**: 代替システムの創発

## メカニズムID

**[T-01] Institutional Substitution** — 機能を担う制度の置換
**[T-02] Paradigm Substitution** — パラダイムの置換
