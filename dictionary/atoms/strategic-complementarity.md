---
id: "strategic-complementarity"
name: "戦略的補完性"
type: "atom"
domain: "economic"
created: 2026-04-29
---

# 戦略的補完性

ある主体の最適行動が、他の主体の行動に**強く依存**する利得構造。「他者が協力するなら自分も協力、他者が裏切るなら自分も裏切る」型の利得関数。

## 起源（Why this exists）

経済・社会のシステムには、ネットワーク効果・採用効果・信頼効果などにより、**他者の行動が自分の利得を変える**構造が頻出する。新技術採用、銀行取り付け、政治運動への参加、すべて「他者が動くなら自分も動く」が合理的行動になる。

これは個人の意思決定ではなく、**利得関数そのもの**の特性。利得関数が補完性を持つとき、複数の均衡が同時に存在しうる（全員協力 / 全員裏切り）。どちらに収束するかは、初期条件と期待形成で決まる。

このatomがあるからこそ、coordination-failure（劣位均衡へのロックイン）が成立する。

## 観察可能なproxy

- 個人意思決定の遅延（他者の動きを待つ）
- 「みんなが動けば自分も動く」発話
- 採用率と採用速度の非線形関係（閾値前後の急変）
- 銀行取り付け、株式市場のパニック売り

## 介入点（Disable conditions）

- 戦略的補完性の弱化（個人が独立に利得を得られる構造）
- 政府・大企業による「先導者」役割
- 確実な保証（「誰もが動く」と信じられるシグナル）
- 強制的同期（全員一斉開始）

## 関与パターン

- [coordination-failure](../patterns/coordination-failure.md) — 劣位均衡を可能にする利得構造
- （拡張候補: network-effect, prisoners-dilemma, cascade）

## 補足

prisoners-dilemma との違い:
- **prisoners-dilemma**: 支配戦略は裏切り（[dominant-defection]）。協力均衡が一意に存在しない
- **coordination-failure**: 複数均衡が存在（[strategic-complementarity]）。協力均衡も裏切均衡も可能、どちらに行くかが問題

前者はインセンティブの問題、後者は期待の問題。脱出策も異なる。前者は契約やコミットメント装置、後者は焦点化やリーダーシップ。

coordination-failure は **strategic-complementarity × common-knowledge-gap × focal-point-absence** の積。利得構造×情報×制度の三層。
