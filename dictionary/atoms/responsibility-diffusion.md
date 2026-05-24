---
id: "responsibility-diffusion"
name: "責任拡散"
type: "atom"
domain: "social"
created: 2026-04-29
---

# 責任拡散

複数の関係者が存在することで、**個人の責任感が薄まる**集団動態。「他の誰かが対応するだろう」という認知が全員に発生し、結果として誰も対応しない。

## 起源（Why this exists）

Latané & Darley（1968）の傍観者効果実験で実証された社会心理学的現象。人数が増えるほど、各個人の「自分が動く必要性」の認知は反比例で低下する。

これは進化的に、群れの中での役割分担（誰かが警戒、誰かが食糧探索）として機能してきたメカニズムの副作用。役割が明確な場合は機能するが、**役割が曖昧で全員が「誰かが対応すべき」と思う状況**では、責任が宙吊りになる。

組織化・官僚化・大規模化が進むほど、責任拡散は構造的に強まる。

## 観察可能なproxy

- 集団内で問題が認識されてから対応されるまでの時間
- 「誰が責任者か」の質問に答えられない状態
- 「これは私の担当ではない」発話の頻度
- 緊急時のリーダー不在現象

## 介入点（Disable conditions）

- 個別指名（「○○さん、これお願い」と名指す）
- 責任主体の制度化（単一責任者制、RACI マトリクス）
- 集団規模の縮小（小チーム化）
- 「全員の責任」の禁止（「全員」は「誰でもない」と等価）

## 関与パターン

- [bystander-economics](../patterns/bystander-economics.md) — 傍観の社会的根拠
- （拡張候補: groupthink, coordination-failure, judgment-evaporation）

## 補足

[responsibility-aversion]（既存）との違い:
- **responsibility-aversion**: 個人内の動機（負いたくない欲求）
- **responsibility-diffusion**: 集団内の構造（薄まる感覚）

前者は個人心理、後者は集団動態。両者は同時発生しうるが独立。集団規模が大きいほど後者が強まり、前者と組み合わさって傍観が完成する。

bystander-economics の三atom構成：[action-cost-asymmetry]（経済）×[prevention-invisibility]（認知）×[responsibility-diffusion]（社会）。
