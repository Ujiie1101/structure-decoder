---
id: "authority"
name: "権威"
grammar_type: "emergence"
mechanism_id: "E-012"
created: 2026-03-11
---

# authority（権威）

特定の主体・制度・伝統が、正当性と影響力を認められる構造。

## 定義

ある主体が他者の行動・信念・価値判断に対して、強制によらず影響を与える能力を獲得する。権威は承認に基づき、専門性・伝統・カリスマ・制度的地位などから生じる。

## 構造

```
authority_source (expertise/tradition/charisma/office)
  → recognition (by relevant community)
    → legitimacy
      → influence_without_coercion
        → authority_maintenance/erosion
```

## 発動条件

1. 権威の源泉（知識・伝統・カリスマ・制度）
2. 認知する共同体の存在
3. 正当性を支える言説
4. 権威行使の機会

## 失敗条件

- **信頼喪失**: スキャンダル・失敗による崩壊
- **競合**: 代替的権威の出現
- **世代交代**: 新世代による承認拒否
- **過剰行使**: 権威の濫用による反発

## 適用事例

| Layer | Entities |
|-------|----------|
| art | canon, critic |
| technology | standards-body, thought-leader |
| economics | rating-agency, expert-opinion |
| politics | supreme-court, elder-statesman |
| religion | clergy, sacred-text |

## 関連パターン

- **institutionalization**: 権威の制度化
- **persistence**: 権威の時間的持続
- **revival**: 伝統的権威の復興

## メカニズムID

**[AU-01] Epistemic Authority** — 知識・専門性に基づく権威
**[AU-02] Traditional Authority** — 伝統・慣習に基づく権威
