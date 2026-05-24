---
id: "reciprocity-norm"
name: "互恵規範"
type: "atom"
domain: "evolutionary"
created: 2026-04-29
---

# 互恵規範

「受けた恩は返す／受けた害は返す」という、人類に普遍的な規範。直接互恵（tit-for-tat）と間接互恵（評判経由）の両方を含む。

## 起源（Why this exists）

Robert Trivers（1971）が定式化した **reciprocal altruism**（互恵的利他）は、血縁関係を超えた協力を可能にした進化的メカニズム。同じ相手と繰り返し取引する状況（反復ゲーム）では、互恵戦略（tit-for-tat）が支配戦略となる（Axelrod 1984 の computer tournament で実証）。

人類は反復ゲーム環境で進化したため、**「返さない者は罰する」**という直感が脳に組み込まれている。この直感は、契約・法・市場が登場する以前から、社会協力の基盤として機能してきた。

副作用として、現代の**一回限り取引**や**匿名取引**では、互恵直感が誤発火する（恩を返せない相手にも返したくなる、害を受けた相手に過剰に報復する）。

## 観察可能なproxy

- 「恩を返せていない」「借りを返したい」発話の頻度
- 贈与経済の継続（プレゼント、奢り、招待の循環）
- 報復行動のエスカレーション
- 一回限り取引での過剰な信頼（観光地の被害）
- 評判メカニズムの強さ

## 介入点（Disable conditions）

- 反復化（一回限りを継続関係に変換）
- 評判システム（間接互恵の制度化）
- 強制力（互恵に依存しない契約執行）
- 互恵の透明化（誰が誰に何を返すかの可視化）

## 関与パターン

- [prisoners-dilemma](../patterns/prisoners-dilemma.md) — 反復化での脱出条件として作動
- [coordination-failure](../patterns/coordination-failure.md) — 焦点形成の補助
- （拡張候補: revenge-spiral, gift-economy, tit-for-tat-cooperation）

## 補足

このatomは進化的に深く埋め込まれているため、**消すことはできない**。むしろ正しい方向に活用する atom。

現代社会の多くの制度（評判システム、SNSのいいね、プラットフォームの星評価）は、互恵規範を**人工的に間接化**して機能させている。Uber 評価、Amazon レビュー、信用スコア──すべて互恵直感を制度化した拡張形。

[non-iteration]（既存、prisoners-dilemma で使用）と裏表の関係。non-iteration は互恵を**機能させなくする**条件、reciprocity-norm は互恵が**働く**前提。
