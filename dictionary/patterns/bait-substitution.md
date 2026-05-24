---
id: "bait-substitution"
name: "餌の置き換え攻撃"
grammar_type: "transformation"
created: 2026-05-13
source_work: "夏目漱石『坊っちゃん』第八章（うらなりを延岡へ追いやり、その差額を坊っちゃんの増給として提示する赤シャツ）"
composition:
  - atom: kindness-intrusion
    role: 親切の文法で提示される
  - atom: arsonist-firefighter-identity
    role: 排除した本人が分配する
---

# bait-substitution（餌の置き換え攻撃）

Aを排除する代わりに、**Aの周辺にいるBにAの利益の一部を回す**装置。Bが受け取った瞬間に、Bは加害の共犯になる。

## 定義

四項構造:

1. **被排除者A**: 強制転任・解雇・降格など
2. **共犯候補B**: Aの隣にいる、独立した立場の人物
3. **餌**: Aの利益の一部（給与差額・席・権限）がBに提示される
4. **提示者C**: Aを排除した張本人がBに餌を渡す

数字上は「誰も損していない」Win-Win構造に見える。だが構造的にはAの排除なしには成立しない取引。

## 構造

```
A_removal（Aの強制排除）
  → resource_redirection（Aの資源をBに振替）
    → kindness_framing（Bへの『親切』として提示）
      → complicit_acceptance（Bが受け取る）
        → cooperative_silence（Bは以後Cの排除を黙認する）
```

## 観察可能な現代具体例

- 早期退職パッケージで他人の枠を埋めて昇進する人事
- 競合の倒産で得た顧客で売上を伸ばす営業
- 被害者報道で得たアクセス数で稼ぐメディア
- リストラ後の残留社員への昇給
- 部署統合での「お互いに業務効率化」型の人員整理

## 対抗装置

- 餌の財源を追う（「この昇給はどこから来た？」を最低3段階遡る）
- [frontal-method-purity](../atoms/frontal-method-purity.md) — 排除された側に立つ
- 「Win-Win」と称される取引で**消えた四人目**を探す習慣

## 関連パターン

- [un-accusable-attack](un-accusable-attack.md) — 上位メタパターン
- [kindness-intrusion](../atoms/kindness-intrusion.md) — 提示の言語形態
- [externalization-cascade](externalization-cascade.md) — コストの外部化との対比
