---
id: "action-cost-asymmetry"
name: "行動コスト非対称"
type: "atom"
domain: "economic"
created: 2026-04-29
---

# 行動コスト非対称

「行動する」と「行動しない」の間に存在する、構造的なコスト非対称。多くの場合、**傍観のほうが圧倒的に安く、行動には経費・リスク・責任が伴う**。

## 起源（Why this exists）

行動は資源を消費する：時間、エネルギー、社会的資本、金銭、評判。傍観はこれらを消費しない（少なくとも一見）。経済学的に合理的な個人は、コストの低い選択を取る傾向がある。

特に、行動の便益が**間接的・統計的・遅延的**な場合（被害の予防、長期改善）、コストは現在で発生し、便益は未来で実現する。時間割引も合わさり、行動は二重に不利になる。

これは個人のずるさではなく、コスト構造そのものから導かれる。

## 観察可能なproxy

- 警告システムへの対応率（応答 vs 無視の比率）
- 「対応する余裕がない」という発話頻度
- 内部告発者のキャリア追跡（罰されている率）
- 行動コストの可視化レベル vs 傍観コストの可視化レベル

## 介入点（Disable conditions）

- 行動コストの低減（自動化、ツール提供、報告経路の簡素化）
- 傍観コストの上昇（法的責任、評判リスク、罰則）
- 行動の評価制度化（「行動した」を昇進評価に組み込む）
- 集合行動化（一人で行動するのではなく集団で）

## 関与パターン

- [bystander-economics](../patterns/bystander-economics.md) — 傍観の経済的根拠
- （拡張候補: moral-hazard, collective-action-problem, output-less-critique）

## 補足

このatomは [responsibility-aversion]（既存）と隣接するが別物。
- **responsibility-aversion**: 個人の心理（負いたくない欲求）
- **action-cost-asymmetry**: 環境の構造（コスト分布）

前者は本人の感情、後者は本人外の経済構造。両者は組み合わさることが多いが、独立して発動する。

bystander-economics は **action-cost-asymmetry × prevention-invisibility × responsibility-diffusion** の積。経済 × 認知 × 社会の三層。
