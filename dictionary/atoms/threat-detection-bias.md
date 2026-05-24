---
id: "threat-detection-bias"
name: "脅威検知バイアス"
type: "atom"
domain: "evolutionary"
created: 2026-04-29
---

# 脅威検知バイアス

潜在的脅威に対して**過剰反応**する認知傾向。誤検知（false positive）のコストが、見落とし（false negative）のコストより**圧倒的に低い**ため、進化的に偽陽性方向に偏った検知が選択された。

## 起源（Why this exists）

Smoke Detector Principle（Nesse 2005）：捕食者検知システムにおいて、見落としは死、誤検知は走る無駄。コスト非対称が極端なため、自然選択は **過剰検知** を強化した。

これは個別の能力ではなく、**全人類共通の認知設計**。動く影、暗闇、孤立、知らない顔──これらすべてに過剰反応するように脳は配線されている。Joseph LeDoux の amygdala 研究で神経科学的にも実証。

副作用として、現代の非脅威に対する誤発火が頻発する：
- 異質な集団への警戒（外国人、新参者、違う見た目）
- 統計的には安全な状況での過剰恐怖（飛行機、原発）
- メディア報道される稀な事件への過剰反応（連れ去り、テロ）

## 観察可能なproxy

- 統計的リスクと主観的恐怖の乖離（飛行機 vs 自動車）
- 「念のため」発話の頻度
- 異質性への即時警戒反応
- ニュース消費後の不安水準上昇
- 楽観的予測より悲観的予測を信じやすい傾向

## 介入点（Disable conditions）

- 統計教育・確率思考の訓練
- 慣れによる脱感作（exposure therapy 的アプローチ）
- メディアダイエット
- 「不安は誤発火である」というメタ認知

## 関与パターン

- [chilling-effect](../patterns/chilling-effect.md) — identification-mirror（自己投影）の進化的下地
- [exemplary-visibility](../patterns/chilling-effect.md) — 見せしめが効く神経的根拠
- [prisoners-dilemma](../patterns/prisoners-dilemma.md) — 「先に裏切られる」恐怖の根拠
- （拡張候補: stranger-danger, in-group-bias の補完）

## 補足

このatomは [identification-mirror]（既存、chilling-effect で使用）の**進化的下地**。identification-mirror は「他人事を自分事として処理する」認知操作だが、なぜそうなるかは threat-detection-bias で説明できる。**他人の被害を見て自分も警戒する**のは、進化的に最適だった。

現代の SNS 時代では、threat-detection-bias が**情報環境**で誤発火し続ける。地球の反対側の脅威を24時間届けられる環境は、進化的に想定されていない。結果として、人類史上最も安全な時代に、人類史上最も不安な人々が生まれている。
