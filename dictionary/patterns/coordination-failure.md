---
id: "coordination-failure"
name: "協調失敗"
grammar_type: "emergence"
mechanism_id: "E-030"
created: 2026-03-11
composition:
  - atom: strategic-complementarity
    role: 他者の行動が自分の利得を決める利得構造
  - atom: common-knowledge-gap
    role: 「全員が知っている」を全員が確信できない高階情報の不在
  - atom: focal-point-absence
    role: 自然な収斂点（Schelling focal point）の不在
composition_formula: "strategic-complementarity × common-knowledge-gap × focal-point-absence"
composition_note: "利得構造（経済） × 期待形成（社会） × 脱出機構（制度）の三層。prisoners-dilemma がインセンティブ問題（裏切りが支配戦略）であるのに対し、coordination-failure は期待問題（協力均衡も裏切均衡も可能）。三者揃って劣位均衡にロックインされる。"
---

# coordination-failure（協調失敗）

各主体が合理的に行動しても、全体として非効率な均衡に陥る構造。

## 定義

複数の主体が相互に依存する状況で、コミュニケーションや調整メカニズムの欠如により、全員がより良い結果を望んでいるにもかかわらず、劣った均衡から脱出できない状態。

## 構造

```
multiple_equilibria_exist
  → agents_lack_coordination_mechanism
    → expectations_mismatch
      → lock_in_to_inferior_equilibrium
        → collective_loss (despite individual rationality)
```

## 発動条件

1. 複数均衡の存在
2. 行動が他者の行動に依存（戦略的補完性）
3. 共有知識・共通期待の欠如
4. 調整装置（focal point）の不在

## 脱出条件

- **focal point**: 自然な調整点の存在
- **cheap talk**: 低コストのコミュニケーション
- **リーダーシップ**: 調整を促すアクター
- **制度設計**: 明示的な調整メカニズム

## 適用事例

| Layer | Entities |
|-------|----------|
| economics | bank-run, currency-crisis, technology-adoption |
| politics | collective-action-problem, voting-paradox |
| technology | network-effects, platform-lock-in |
| history | league-of-nations, eurozone-crisis |

## 関連パターン

- **prisoners-dilemma**: インセンティブ問題 vs 調整問題
- **cascade**: 調整失敗からの連鎖的崩壊
- **emergence**: 調整成功時の自発的秩序

## 注意

囚人のジレンマとは異なり、協調失敗では「全員が協力したい」が「誰が先に動くか」の問題。インセンティブ問題ではなく期待形成問題。
