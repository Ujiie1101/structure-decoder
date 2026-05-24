---
id: "commitment-impossibility"
name: "コミットメント不能"
type: "atom"
domain: "institutional"
created: 2026-04-29
---

# コミットメント不能

将来の行動を**強制的に拘束する手段**が存在しない状態。「協力する」と約束しても、実行段階で破ることが可能。

## 起源（Why this exists）

人間は将来の自分の行動を約束できる。しかし約束は、約束時点では実行されていない。実行段階に達したとき、その時点での状況や利害に応じて約束を破ることは原理的に可能。

約束を強制力に変換するには、外部装置が必要：契約と裁判所、評判と社会的記憶、抵当と差し押さえ、組織と懲戒、宗教と神罰。これらの装置がない or 機能しない状況では、約束は単なる発話で終わる。

国際関係、新興市場、非公式な取引、技術が急変する領域、では強制装置が脆弱になりがち。結果として commitment-impossibility が常態化する。

## 観察可能なproxy

- 契約執行の実効性（裁判所の機能度）
- 評判メカニズムの作動度（再取引の可能性、ネットワーク密度）
- 第三者保証の存在
- 過去の約束破りに対する罰の事例数

## 介入点（Disable conditions）

- 制度的拘束装置（契約、抵当、保証金）
- 評判メカニズムの強化（記録、共有、長期取引）
- 段階的取引（小さな約束を積み重ねて信頼を構築）
- 一方的コミットメント（自らの選択肢を物理的に削除する）

## 関与パターン

- [prisoners-dilemma](../patterns/prisoners-dilemma.md) — ジレンマの脱出阻害要因
- （拡張候補: tragedy-of-commons, time-inconsistency, hold-up-problem）

## 補足

[sunk-commitment] と区別が重要:
- **sunk-commitment**: 過去の投入が現在の決定を縛る（撤退不能）
- **commitment-impossibility**: 将来の行動を約束できない（前進不能）

前者は「もう引き返せない」、後者は「進めると約束できない」。時間方向が逆。両者とも合理的選択を妨げるが、構造は反対。

prisoners-dilemma を脱出する試みのほとんどは commitment-impossibility を打破する制度設計（contracts, repeated games, reputation systems）。これらが機能しない領域でだけ、ジレンマは構造化された罠として残る。
