---
id: "triangulation-attack"
name: "三角測量攻撃"
grammar_type: "transformation"
created: 2026-05-13
source_work: "夏目漱石『坊っちゃん』第五章（『磊落・淡泊・親切に下宿の世話』で山嵐を名指さずに名指す赤シャツ）"
composition:
  - atom: adjective-arrow
    role: 直接攻撃を回避する言語装置
  - atom: responsibility-aversion
    role: 解釈責任を聞き手に転移させる
---

# triangulation-attack（三角測量攻撃）

攻撃者が**直接相手を攻撃せず、第三者の口を借りる**、または**一般論の形で攻撃の輪郭だけを描き、固有名は受け手の側に補完させる**装置。攻撃の責任は語った側ではなく解釈した側に移る。

## 定義

攻撃が以下の構造を持つ:

1. **語り手A**: 一般論・形容詞・第三者の発言として攻撃の輪郭を描く
2. **解釈者B**: 自分の記憶・知識と照合して、攻撃対象Cを補完する
3. **対象C**: 攻撃を受けるが、Aは「私は名指していない」と否認可能

攻撃の責任が、語り手A → 解釈者Bに移される。Bは「自分の判断で攻撃対象を補完した」と認知する。

## 構造

```
general_statement（一般論を発する）
  → listener_completion（聞き手が固有名を補完）
    → cognitive_ownership（聞き手は『自分の判断』と認知）
      → speaker_deniability（語り手は名指しを否認できる）
        → attack_lands_invisibly（攻撃は不可視で着弾）
```

## 観察可能な現代具体例

- 「世の中には磊落なように見えても油断できない人がいる」
- 「これは一般論だけど、ある業界では……」
- 「人を信用しすぎる人はリスクが高い」
- ハラスメント研修で「こういう傾向がある人もいるので皆さんお気をつけて」

## 対抗装置

- [frontal-method-purity](../atoms/frontal-method-purity.md) — 自分から名指す
- 即座の補完拒否（「で、具体的に誰のことですか」）
- 一般論の論理的整合性のみを検証し、人物への補完を停止する

## 関連パターン

- [un-accusable-attack](un-accusable-attack.md) — 上位メタパターン
- [innuendo-broadcast](innuendo-broadcast.md) — 第三者前の運用
- [bait-substitution](bait-substitution.md) — 経済形態への応用
