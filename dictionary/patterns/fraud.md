---
id: "fraud"
name: "詐欺"
grammar_type: "emergence"
mechanism_id: "E-058"
layer: 3
domains: ["technology"]
created: 2026-03-11
---

# fraud（詐欺）

虚偽の情報で相手を欺き、不正な利益を得る構造。

## 定義

意図的な虚偽表示、隠蔽、操作によって、被害者の判断を誤らせ、財産・信頼・機会を詐取する。情報の非対称性を悪用し、発覚までの時間差を利用する。

## 構造

```
information_asymmetry
  → false_representation
    → victim_deception
      → resource_extraction
        → concealment / collapse
```

## 発動条件

1. 情報の非対称性
2. 被害者の信頼・欲望
3. 検証困難な主張
4. 発覚遅延の仕組み

## 失敗条件

- **発覚**: 検証・内部告発
- **持続不能**: ポンジー構造の限界
- **規制強化**: 監視・罰則の厳格化
- **評判崩壊**: 信頼ネットワークからの排除

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | phishing, deepfake, crypto-scam |
| economics | ponzi-scheme, enron, theranos, madoff |
| history | south-sea-bubble, tulip-mania |
| philosophy | sophistry, bad-faith |
| society | identity-theft, corporate-fraud |

## 関連パターン

- **information-asymmetry**: 詐欺の前提条件
- **cascade**: 詐欺発覚後の連鎖崩壊
- **trust**: 信頼の濫用と破壊
- **collapse**: 詐欺スキームの必然的崩壊
