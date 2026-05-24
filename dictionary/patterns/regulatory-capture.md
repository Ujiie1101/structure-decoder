---
id: "regulatory-capture"
name: "規制の虜"
grammar_type: "emergence"
mechanism_id: "E-119"
created: 2026-03-11
---

# regulatory-capture（規制の虜）

規制機関が規制対象の利益のために機能するようになる構造。

## 定義

公益のために設立された規制機関が、情報の非対称性・人材交流・ロビー活動などにより、規制対象産業の利益を優先するようになり、本来の機能を喪失する。

## 構造

```
regulatory_agency (public interest mandate)
  → information_asymmetry
    → industry_expertise_dependence
      → revolving_door
        → captured_regulation (serves regulated industry)
```

## 発動条件

1. 専門知識の産業側集中
2. 規制当局と産業の継続的接触
3. 人材の相互流動（回転ドア）
4. 規制対象のロビー資源

## 失敗条件

- **透明性**: 規制プロセスの可視化
- **独立性**: 規制機関の資金・人事の独立
- **多元化**: 多様なステークホルダーの参加
- **スキャンダル**: 癒着の露見による改革

## 適用事例

| Layer | Entities |
|-------|----------|
| economics | financial-regulation, telecommunications |
| technology | fcc, fda, big-tech-regulation |
| history | icc, railroad-regulation |
| philosophy | public-choice-theory |

## 関連パターン

- **principal-agent-divergence**: 規制者と公益の乖離
- **information-asymmetry**: 捕獲の基盤
- **institutionalization**: 捕獲の固定化

## メカニズムID

**[E-01] Invisible Hand Coordination** — 個々の利益追求から規制捕獲が創発
