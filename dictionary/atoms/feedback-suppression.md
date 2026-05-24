---
id: "feedback-suppression"
name: "フィードバック抑圧"
type: "atom"
domain: "institutional"
created: 2026-04-29
---

# フィードバック抑圧

警告・異論・ネガティブな情報が、組織の階層フィルターを通過できず、意思決定者に届かない構造。情報の縦軸（下→上）の遮断。

## 起源（Why this exists）

組織が大きくなるほど、情報は中間層を経由してトップに届く。中間層には自らの保身（悪い知らせを運ぶと不利）と、組織防衛（外に漏らすと組織が損をする）の二重インセンティブが働く。

結果として、ネガティブ情報は中間層で**自動的にフィルター**される。これは個人の悪意ではなく、構造的に発生する選択圧。フィルターを回避する制度（ホットライン、外部監査、whistleblower保護）を意図的に設計しなければ、組織は成長と共に必然的に情報遮断状態に向かう。

## 観察可能なproxy

- トップへの報告書のトーン分析（ポジティブ偏重）
- 中間管理職層の同質性
- 「悪い知らせ」発信者のキャリア追跡
- 外部監査・第三者評価の頻度
- 内部告発の発生率と処遇

## 介入点（Disable conditions）

- 階層を飛び越えるチャネル（skip-level meeting、ホットライン）
- 外部からのインプット（コンサル、監査、研究者）
- ネガティブ情報の構造化要求（pre-mortem、red team review）
- 中間層のインセンティブ再設計（messenger を罰しない明示的ルール）

## 関与パターン

- [hubris-nemesis](../patterns/hubris-nemesis.md) — 警告が届かないから傲慢が修正されない
- （拡張候補: groupthink, mission-drift, expertise-blindness, judgment-evaporation）

## 補足

[dissent-suppression] と区別が重要:
- **feedback-suppression**: 縦軸（下→上の情報フィルター）。組織構造の問題。
- **dissent-suppression**: 横軸（メンバー間の異論抑圧）。集団動態の問題。

両者は同じ組織で同時発生しうるが、独立した別ベクトル。介入策も異なる。前者は構造改革、後者は文化改革。
