---
id: "alternative-cost"
name: "代案コスト"
type: "atom"
domain: "economic"
created: 2026-04-29
---

# 代案コスト

「批判する」と「代案を提示する」の間に存在する、**思考コストと責任コストの非対称**。批判は安く、代案は高い。

## 起源（Why this exists）

代案を提示するには:
1. **問題理解の深さ**（部分批判では足りず、全体把握が必要）
2. **設計能力**（システムを再構築する想像力）
3. **検証責任**（提案が機能するか問われる）
4. **実装コミット**（提案を実現する責任）

一方、批判は問題の一部を指摘するだけで成立する。深い理解も検証責任も実装コミットも要求されない。

経済合理的な発信者は、コストの低い選択（批判のみ）を選ぶ。これは個人の怠惰ではなく、**コスト構造の必然**。

## 観察可能なproxy

- SNS投稿の批判 vs 提案の比率
- 「では何をすべきか」と問われた時の沈黙
- 評論家の代案実装率
- 「批判的思考」教育の広がり vs 「建設的提案」教育の不在

## 介入点（Disable conditions）

- 代案の義務化（批判時に代案を必須にする制度）
- 代案コストの低減（テンプレ提供、参考資料の充実）
- 代案の評価（提案を成果として評価する制度）
- 「批判のみ」を罰する文化（無責任な批判への警戒）

## 関与パターン

- [output-less-critique](../patterns/output-less-critique.md) — 経済的根拠
- （拡張候補: responsibility-aversion, free-riding, stake-free-visibility）

## 補足

[responsibility-aversion]（既存）との違い:
- **responsibility-aversion**: 結果責任を負いたくない動機
- **alternative-cost**: 代案を作る思考・実装コスト

前者は責任の事後的回避、後者は事前的コスト。両者は重なるが独立。代案コストが低くても責任回避は起こりうる（誰かが用意した代案を「自分のもの」と装う）。両者揃うと、output-less-critique が完成する。

output-less-critique の三atom構成：
- [alternative-cost]：思考・実装コスト（経済）
- [empathy-incentive]：共感報酬の構造（社会）
- [stake-free-visibility]：賭けなき可視性（社会）
