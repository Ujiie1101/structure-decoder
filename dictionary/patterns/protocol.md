---
id: "protocol"
name: "プロトコル"
grammar_type: "emergence"
layer: 3
mechanism_id: "E-110"
domains: ["art", "technology"]
created: 2026-03-11
---

# protocol（プロトコル）

相互作用を可能にする合意されたルール・手順の構造。

## 定義

異なる主体・システム間の相互運用を可能にする、形式化された規則・手順・標準。通信プロトコル、社会的規範、芸術的慣習を含む。

## 構造

```
need_for_interoperability
  → protocol_design
    → adoption/agreement
      → standardization
        → enabled_interaction
```

## 発動条件

1. 相互作用の必要性
2. プロトコル設計能力
3. 合意形成メカニズム
4. 遵守のインセンティブ

## 失敗条件

- **不採用**: 普及の失敗
- **競合**: 複数プロトコルの並立
- **硬直化**: 変化への不適応
- **悪用**: プロトコルの逸脱利用

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | tcp-ip, http, blockchain-protocols |
| art | artistic-conventions, musical-notation |
| diplomacy | diplomatic-protocol, international-law |
| society | social-norms, etiquette |

## 関連パターン

- **coordination**: プロトコルによる協調
- **network**: プロトコルが可能にする接続
- **emergence**: プロトコル上の創発
