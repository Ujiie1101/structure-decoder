---
id: "measurable-displacement"
name: "測定可能性の置換"
type: "atom"
domain: "institutional"
created: 2026-04-29
---

# 測定可能性の置換

測定可能な指標が、測定不可能だが本質的な目的を**置き換えてしまう**構造。Goodhart's Law（測定対象は目標化し、目標は歪む）の一般化。

## 起源（Why this exists）

組織は規模が大きくなるほど、暗黙知や定性的判断を伝達するコストが上昇する。代わりに数値化された指標は、メンバー間で同じ意味で共有でき、評価・報酬・昇進の基準にできる。

結果として、測定可能なものへの移行は組織の効率化として進む。しかし測定可能なものは多くの場合、本来の目的の**代理変数（プロキシ）**にすぎない。プロキシが目標化されると、本来の目的への忠実度よりも、プロキシ達成への適合が優先される。

これは個人の悪意ではなく、伝達コストと評価コストの最小化から自動的に発生する。

## 観察可能なproxy

- KPIの数の経年増加
- 「測れるもの」と「測れないもの」の組織内優先度ギャップ
- 数値達成率と本来目的達成感の乖離
- 「指標は達成したが本質を見失った」という事後評価
- 評価制度から定性評価が消えていく

## 介入点（Disable conditions）

- 測定不可能な目的の制度化（mission statement の儀式的再確認）
- プロキシの定期的見直し（指標自体を疑う制度）
- 定性評価の強制化（数値に還元しない判断要求）
- 「測れないが重要」リストの維持

## 関与パターン

- [mission-drift](../patterns/mission-drift.md) — 漂流の主要駆動力
- （拡張候補: goodharts-law, principal-agent-divergence, expertise-blindness）

## 補足

このatomは Goodhart's Law（社会指標は目標化されると指標性を失う）の構造論的記述。Goodhart 自身は経済政策での observation だったが、組織・教育・医療・科学のあらゆる領域で同じ構造が発動する。

mission-drift では **[stakeholder-multiplication] × [founder-distance]** と組み合わさる。多様なステークホルダー（測定要求の発信源）と原点からの距離（測定不能な原点の保護者の不在）が、measurable-displacement を加速する。
