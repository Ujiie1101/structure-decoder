---
id: "prisoners-dilemma"
name: "囚人のジレンマ"
grammar_type: "collapse"
mechanism_id: "C-002"
created: 2026-02-28
composition:
  - atom: dominant-defection
    role: 利得構造で裏切りが個人合理性の最適解になる
  - atom: commitment-impossibility
    role: 将来の行動を強制拘束する装置の欠如
  - atom: non-iteration
    role: 将来の報復が機能しない一回限り構造
composition_formula: "dominant-defection × commitment-impossibility × non-iteration"
composition_note: "経済（利得構造） × 制度（拘束装置） × 時間（反復性）の三軸。dominant-defection だけなら脱出機構（コミットメント、反復）で簡単に回避される。三者揃って初めて構造化された罠になる。"
---

# prisoners-dilemma（囚人のジレンマ）

個人合理性と集団合理性の乖離。各自が最適を追求すると全員にとって最悪の結果に。

## 定義

各プレイヤーが自己利益を最大化する戦略を選択すると、全員が協力した場合より悪い結果（パレート非効率）に陥る構造。

## 構造

```
Player A: Defect dominates Cooperate
Player B: Defect dominates Cooperate
  → Both Defect
    → (D,D) < (C,C) for both
      → Individual rationality ≠ Collective rationality
```

## 利得行列

|   | B: Cooperate | B: Defect |
|---|--------------|-----------|
| A: Cooperate | (3,3) | (0,5) |
| A: Defect | (5,0) | **(1,1)** ← Nash |

## 発動条件

1. 両者に裏切りのインセンティブ（支配戦略）
2. コミットメント不能（約束の強制不可）
3. 一回限りのゲーム（反復なし）
4. 情報の対称性

## 脱出条件

- **反復ゲーム**: 将来の報復が協力を支える
- **コミットメント装置**: 契約、評判、制度
- **社会的選好**: 利他性、公平性
- **コミュニケーション**: 調整の可能性

## 適用事例

| Layer | Entities |
|-------|----------|
| economics | game-theory, price-wars, arms-race |
| politics | international-cooperation, climate-change |
| history | cold-war-arms-race |

## 関連パターン

- **retaliatory-spiral**: 反復囚人のジレンマの動態
- **hubris-nemesis**: 非協力の帰結としての破滅
- **invisible-hand**: 協力が生じる場合の対比

## 注意

現実の人間は完全な利己主義者ではない。行動ゲーム理論は、協力率が理論予測より高いことを示す。
