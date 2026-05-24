---
id: "constraint"
name: "制約"
grammar_type: "constraint"
mechanism_id: "N-001"
created: 2026-03-11
---

# constraint（制約）

自由度を制限することで特定の方向性を生み出す構造。

## 定義

規則・構造・資源制限などが行為者の選択肢を狭め、特定の経路や結果へと誘導する。制約は抑圧にも、創造性の源泉にもなりうる。

## 構造

```
open_possibility_space
  → constraint_introduction
    → option_reduction
      → channeled_behavior
        → path_dependency
```

## 発動条件

1. 制約の存在と認識
2. 制約を回避するコストの高さ
3. 制約内での行動インセンティブ
4. 制約の安定性

## 失敗条件（制約無効化）

- **回避**: 制約を迂回する方法の発見
- **打破**: 制約の除去
- **無視**: 制約コストの受容
- **変容**: 制約条件の変化

## 適用事例

| Layer | Entities |
|-------|----------|
| politics | constitution, separation-of-powers |
| economics | budget-constraint, regulation |
| religion | religious-law, taboo |
| art | form-constraint, genre-rules |
| technology | technical-standards, protocols |

## 関連パターン

- **path-dependency**: 制約による経路固定
- **emergence**: 制約内での創発
- **substitution**: 制約回避のための代替

## メカニズムID

**[F-02] Path Dependency** — 経路依存性
