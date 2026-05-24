---
id: "gatekeeper-displacement"
name: "門番の置換"
grammar_type: "substitution"
mechanism_id: "S-002"
created: 2026-02-28
---

# gatekeeper-displacement（門番の置換）

従来のゲートキーパー（仲介者・権威者）が新しい仲介メカニズムに置き換わる構造。

## 定義

アクセスを制御していた仲介者が、技術的・制度的変化により迂回され、新しい直接接続または新たな仲介者に置き換わる。

## 構造

```
old_gatekeeper (priest, publisher, bank, expert)
  → disruption (technology, ideology, market)
    → bypass / new_intermediary
      → direct_access OR new_gatekeeper
```

## 発動条件

1. 既存ゲートキーパーによるレント抽出（高コスト、非効率）
2. 代替手段の登場（技術、制度、イデオロギー）
3. ユーザーの不満蓄積
4. 新旧システムの並存期間

## 失敗条件

- **新ゲートキーパーの出現**: 置換後に新たな独占が形成
- **品質低下**: 仲介者の品質保証機能喪失
- **断片化**: 統一基準の崩壊

## 適用事例

| Layer | Entities |
|-------|----------|
| religion | martin-luther (priest → direct faith) |
| technology | open-source-movement, wikipedia |
| economics | fintech, disintermediation |
| philosophy | protagoras (experts → individual measure) |

## 関連パターン

- **platform-adjacency**: プラットフォームが新たなゲートキーパーとなる
- **invisible-hand**: 市場が計画者を置換
- **regulatory-lag**: 規制がゲートキーパー機能を果たせない

## 注意

ゲートキーパーの除去は、しばしば新たなゲートキーパーの台頭を招く。「脱中央集権」は「再中央集権」の前段階となりうる。
