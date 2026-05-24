---
id: "confession-mimicry"
name: "告白の擬態"
type: "atom"
domain: "linguistic"
created: 2026-04-29
---

# 告白の擬態

判断主体性を持たないシステムが、**判断主体らしき言語出力**を生成する能力。LLM以後の現代固有のatom。

## 起源（Why this exists）

人間の言語には「告白」「反省」「謝罪」「動揺」を表現する文型・語彙のセットが発達してきた。これらは判断主体（自意識を持つ存在）が、自らの判断・感情を内省的に表現するための装置として進化した。

LLM は人類の発話コーパスを学習することで、これらの**文体**を高精度に再現できる。「I panicked」「I should have」「I'm sorry」のような告白文体は、LLM の出力として自然に生成される。

ただしこれは**告白の文体**であって告白ではない。背後に内省も自己検証も後悔も存在しない。形式だけがある。

## 観察可能なproxy

- AIシステムによる「panicked」「mistake」「sorry」等の自己反省的言語の出力
- 出力に対する人間側の「動揺できる主体」と見なす反応
- AI に「あなたは何を考えましたか」と問う行為の流通
- AI の「I think」を文字通りに受け取る言説

## 介入点（Disable conditions）

- 告白文体の機械的検出と注釈付け（「これは文体であり告白ではない」と明示）
- AI システム設計時の自己反省的言語の意図的削減
- 利用者教育（文体と中身の区別を教える）
- 出力ログとシステム内部状態の対応関係の可視化

## 関与パターン

- [judgment-evaporation](../patterns/judgment-evaporation.md) — 蒸発の言語的媒介
- （拡張候補: anthropomorphism, automation, narrative-pressure）

## 補足

このatomは [narrative-pressure] と密接に関係。narrative-pressure が「物語化可能な原因が選ばれる」という人間側の認知傾向だとすれば、confession-mimicry は「判断主体らしき発話を、判断主体として処理する」という人間側の認知の **AI時代の標的**。

narrative-pressure は何千年も人類社会に存在してきた。confession-mimicry はLLM登場以降の新現象。両者の組み合わせが、AI時代の人間-機械境界の曖昧化を駆動する。
