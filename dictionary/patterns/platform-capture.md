---
id: "platform-capture"
name: "プラットフォーム捕獲"
grammar_type: "emergence"
mechanism_id: "E-100"
created: 2026-03-11
---

# platform-capture（プラットフォーム捕獲）

プラットフォームが参加者を依存状態に置き、価値を吸い上げる構造。

## 定義

プラットフォームは初期に参加者に価値を提供してエコシステムを構築するが、臨界質量到達後は支配的地位を利用して参加者の余剰を捕獲する。「育てて、囲い込み、収穫する」サイクル。

## 構造

```
platform_launch (value_offering)
  → ecosystem_growth
    → dependency_creation (lock-in, switching_cost)
      → surplus_extraction
        → captured_value (platform takes disproportionate share)
```

## 発動条件

1. ネットワーク効果の存在
2. 参加者のスイッチングコスト
3. 情報非対称性（プラットフォームが全データを把握）
4. 代替プラットフォームの不在

## 失敗条件

- **過剰搾取**: 参加者離反による崩壊
- **マルチホーミング**: 複数プラットフォーム併用
- **規制介入**: 相互運用性義務、分割
- **技術的破壊**: 分散型代替の出現

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | app-store-30percent, amazon-marketplace, google-adsense |
| economics | visa-mastercard, real-estate-platforms |
| history | colonial-trading-companies, medieval-guilds |
| art | streaming-platforms, gallery-system |

## 関連パターン

- **emergence**: プラットフォームからエコシステムが創発
- **network-effect**: 捕獲の前提条件
- **extraction**: 価値抽出パターン
- **platform-adjacency**: 隣接市場への拡張

## メカニズムID

**[E-03] Platform Rent-Seeking** — プラットフォーム支配から参加者余剰の捕獲が生じる
