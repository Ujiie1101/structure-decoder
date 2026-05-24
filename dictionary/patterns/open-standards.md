---
id: "open-standards"
name: "オープン標準"
grammar_type: "emergence"
mechanism_id: "E-093"
created: 2026-03-11
---

# open-standards（オープン標準）

公開され、誰でも実装可能な技術仕様により相互運用性を実現する構造。

## 定義

特定の企業・組織が排他的に管理しない、公開された技術仕様に基づき、異なる実装間の互換性・相互運用性を確保し、イノベーションと競争を促進する仕組み。

## 構造

```
interoperability_need
  → specification_development
    → open_publication
      → multiple_implementations
        → network_growth (innovation on shared foundation)
```

## 発動条件

1. 相互運用性への需要
2. 標準化プロセスの透明性
3. 実装の自由（ライセンス）
4. 十分な採用（クリティカルマス）

## 失敗条件

- **分裂**: 競合標準による断片化
- **捕獲**: 特定企業による標準の私物化
- **停滞**: 標準化プロセスの硬直化
- **無視**: デファクト標準による回避

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | tcp-ip, html, http, usb, bluetooth |
| economics | iso-standards, accounting-standards |
| history | railroad-gauge, electrical-standards |
| philosophy | public-goods, commons |

## 関連パターン

- **network-effect**: 標準採用のネットワーク効果
- **coordination**: 標準による協調
- **decentralization**: 標準による分散化

## メカニズムID

**[E-01] Invisible Hand Coordination** — 分散的採用決定から共通基盤が創発
