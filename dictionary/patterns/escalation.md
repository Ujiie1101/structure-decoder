---
id: "escalation"
name: "エスカレーション"
grammar_type: "emergence"
mechanism_id: "E-049"
created: 2026-03-11
composition:
  - atom: intent-uncertainty
    role: 相手の防衛的行動を攻撃的と誤読させ、過剰反応を呼ぶ
  - atom: face-investment
    role: 公開された対立で撤退路を閉ざす
  - atom: sunk-commitment
    role: 投入資源が増えるほど撤退コストを上げ、さらなる投入を呼ぶ
composition_formula: "intent-uncertainty × face-investment × sunk-commitment"
composition_note: "誤読（intent-uncertainty）は引き金、face-investment は公的撤退路の封鎖、sunk-commitment は機械的不可逆性。三層が独立に作用する。"
---

# escalation（エスカレーション）

相互作用により対立・緊張・手段が段階的に激化する構造。

## 定義

二者以上のアクター間の相互反応が、各ステップでより強い対応を創発させ、当初の意図を超えた激化に至る。誰も意図しない結果が、相互作用の論理から不可避的に生じる。

## 構造

```
initial_tension
  → action_by_party_A
    → perceived_provocation
      → escalated_response_by_party_B
        → further_escalation
          → crisis_or_rupture (emergent unintended outcome)
```

## 発動条件

1. 相互依存的な対立構造
2. 相手の意図の誤認
3. 面子・威信の投入
4. 撤退コストの増大

## 失敗条件

- **脱エスカレーション**: 意図的な緊張緩和
- **仲介者**: 第三者による介入
- **疲弊**: 双方のリソース枯渇
- **枠組み変更**: 対立軸の再定義

## 適用事例

| Layer | Entities |
|-------|----------|
| politics | arms-race, trade-war, diplomatic-crisis |
| history | july-crisis-1914, cuban-missile-crisis |
| economics | price-war, regulatory-retaliation |
| psychology | conflict-spiral, grudge-match |
| technology | cyber-escalation |

## 関連パターン

- **mutual-checking**: エスカレーション抑止
- **cascade**: エスカレーションの連鎖的拡大
- **retaliatory-spiral**: 報復エスカレーション

## メカニズムID

**[E-07] Security Dilemma** — 安全保障のジレンマ
**[E-08] Commitment Trap** — コミットメントの罠
