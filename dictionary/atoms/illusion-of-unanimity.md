---
id: "illusion-of-unanimity"
name: "全員一致の幻想"
type: "atom"
domain: "cognitive"
created: 2026-04-29
---

# 全員一致の幻想

集団内で異論を持つメンバーが沈黙したとき、他のメンバーが「沈黙＝同意」と解釈する集合的錯覚。

## 起源（Why this exists）

人間は他者の心的状態を直接観察できない。可視化されない意見は存在しないものとして処理される（不在の知覚は存在の知覚より遥かに弱い）。

加えて、自分が異論を持って沈黙している場合、その自己経験を他者にも投影することは難しい。他者が沈黙していると、本人は「同意している」とデフォルト解釈する。

つまり全員が異論を持っていても、全員が沈黙していれば、全員が「自分以外は同意している」と思い込む状態が成立しうる。これは pluralistic ignorance（多元的無知）として知られる現象。

## 観察可能なproxy

- 匿名投票と公開合意の乖離
- 解散後の私的会話で吐露される異論
- 後日の振り返りでの「実は反対だった」発言
- 一致決定の自己記述（「全員が同じ考えだった」）

## 介入点（Disable conditions）

- 匿名意見集約（事前匿名投票、匿名チャット）
- 異論の制度化（必ず誰かが異論を出す役割）
- 個別ヒアリング（一対一で意見を聞き出す）
- 「沈黙は同意ではない」ルールの明示化

## 関与パターン

- [groupthink](../patterns/groupthink.md) — 集団の自己誤認を生む
- （拡張候補: emperor's-new-clothes, herd-behavior, normalization）

## 補足

このatomは [conformity-pressure] と [dissent-suppression] の**結果**として発生するが、独立した認知メカニズムでもある。両圧力が無くても、単に「他人の心は見えない」というだけで pluralistic ignorance は成立する。

groupthinkの完全形は **conformity-pressure（自分→自分） × dissent-suppression（他者→自分） × illusion-of-unanimity（自分→他者）** の三者が円環を作って自己強化する状態。各atomは独立だが、揃うと相互強化する。
