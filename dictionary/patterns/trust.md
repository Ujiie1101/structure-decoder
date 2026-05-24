---
id: "trust"
name: "信頼"
grammar_type: "emergence"
mechanism_id: "E-147"
layer: 3
domains: ["technology"]
created: 2026-03-11
---

# trust（信頼）

不確実性の下で相手の行動に期待を置くことで、協力が可能になる構造。

## 定義

完全な情報や保証なしに、他者・システム・制度が期待通りに機能すると信じること。取引コストの削減、社会資本の形成、複雑な協力の基盤となる。裏切りリスクと引き換えに協力の便益を得る。

## 構造

```
uncertainty
  → vulnerability_acceptance
    → positive_expectation
      → cooperation_enabled
        → trust_reinforcement / betrayal
```

## 発動条件

1. 不確実性の存在
2. 相互依存関係
3. 期待形成の根拠（評判、制度、関係）
4. 裏切りに対する制裁可能性

## 失敗条件

- **裏切り**: 信頼の濫用
- **過信**: 検証なき信頼
- **不信の連鎖**: 一度の裏切りが全体を崩壊
- **匿名性**: 評判形成の困難

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | ssl, blockchain, digital-signature, zero-trust |
| economics | credit, contract, currency, brand |
| philosophy | social-contract, good-faith |
| society | institution, rule-of-law |
| religion | faith, covenant |

## 関連パターン

- **emergence**: 信頼から社会秩序が創発
- **coordination**: 信頼による協調
- **cascade**: 信頼崩壊の連鎖
- **network-effect**: 信頼ネットワークの価値
