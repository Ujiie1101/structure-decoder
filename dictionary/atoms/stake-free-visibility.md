---
id: "stake-free-visibility"
name: "賭けなき可視性"
type: "atom"
domain: "social"
created: 2026-04-29
---

# 賭けなき可視性

自分が**何のリスクも負わずに**目立つことができる構造。発信のコストは下がり続け、批判は手軽に行えるが、**自分の側の損失リスク**は限りなくゼロに近い状態。

## 起源（Why this exists）

近代以前、発信は印刷・紙面・直接対話を要し、発信者の身元・立場・社会資本が透明だった。批判すれば批判者本人にもリスクが及んだ（評判低下、訴訟、社会的制裁）。

SNS時代以降:
- **匿名アカウント**で身元を隠せる
- **リプライ・引用**で批判が他者の発信に容易に乗せられる
- **アルゴリズム拡散**で発信者本人の社会資本投入なしに目立てる

結果として、**目立つこと**と**賭けること**が分離した。Nassim Taleb の言う「skin in the game」がない発信者が、市場（言論空間）を圧倒的に占有する。

## 観察可能なproxy

- 匿名アカウントの発信比率
- 批判発信者の身元開示率
- 「炎上」を起こした側のキャリア追跡
- 訴訟リスクの実際の発生率

## 介入点（Disable conditions）

- 発信者の身元紐付け（実名制、認証バッジ）
- 賭けの強制（提案には実装責任、批判には反論受諾義務）
- skin-in-the-game の制度化
- 匿名発信の信頼度低下化（プラットフォーム設計）

## 関与パターン

- [output-less-critique](../patterns/output-less-critique.md) — 賭けの不在による不均衡
- （拡張候補: chilling-effect, exemplary-visibility, hubris）

## 補足

[exemplary-visibility]（既存、chilling-effect で使用）との対比:
- **exemplary-visibility**: 制裁対象の可視性（受け手側の見せしめ）
- **stake-free-visibility**: 発信者の賭けなき可視性（発信者側の無リスク）

両者は対をなす。chilling-effect は「目立つと罰せられる」、stake-free-visibility は「目立っても罰されない」。SNS時代は、**両者が同じプラットフォーム上で同時発生**する不思議な構造を生んでいる。匿名で批判する側は stake-free、実名で発信する側は exemplary という非対称。

output-less-critique の三atom：
- [alternative-cost]：代案を作る経済コスト
- [empathy-incentive]：共感を集める社会報酬
- [stake-free-visibility]：賭けなき発信の社会構造

経済 × 報酬 × 構造の三層独立。
