---
id: "broadcast"
name: "放送・拡散"
grammar_type: "emergence"
mechanism_id: "E-019"
created: 2026-03-11
---

# broadcast（放送・拡散）

情報・コンテンツが一点から多数へ同時に伝達される構造。

## 定義

単一の発信源から不特定多数の受信者へ、同一の情報やコンテンツが同時に配信される。受信者は受動的に情報を受け取り、スケールメリットにより配信コストが逓減する。

## 構造

```
single_source
  → encoding_transmission
    → distribution_network
      → mass_reception
        → cultural_synchronization
```

## 発動条件

1. 大規模配信インフラの存在
2. コンテンツの複製可能性
3. 受信デバイスの普及
4. 同時性への需要

## 失敗条件

- **断片化**: 受信者の注意が分散
- **規制**: 放送免許・検閲による制約
- **技術的限界**: 帯域・到達範囲の制限
- **双方向化**: 一方向モデルの陳腐化

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | radio, television |
| economics | mass-advertising, viral-marketing |
| politics | propaganda, public-address |
| religion | televangelist, mass-prayer |
| art | concert-broadcast, live-streaming |

## 関連パターン

- **network-effects**: 放送が普及を加速
- **standardization**: 放送がコンテンツを均質化
- **commercialization**: 放送が広告モデルを生む

## メカニズムID

**[B-01] One-to-Many Transmission** — 単一発信源から多数受信者への情報伝達
**[B-02] Synchronous Reception** — 同時受信による文化的同期
