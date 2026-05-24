---
id: "labeling-cascade"
name: "ラベリング連鎖"
grammar_type: "transformation"
mechanism_id: "T-045"
created: 2026-03-25
---

# labeling-cascade（ラベリング連鎖）

中立的な表現が連想の連鎖により政治的ラベルに変換され、攻撃対象になる構造。

## 定義

本来は中立的・普遍的な表現が、連想・推論の連鎖を経て特定の政治的立場を示すラベルに変換され、最終的に攻撃の正当化に至る現象。各ステップの飛躍は小さいが、連鎖全体では「平和を願う人」が「敵」になる。

## 構造

```
neutral_expression（中立的表現）
  → association_step_1（連想1）
    → political_label（政治的ラベル）
      → stigmatization（烙印化）
        → enemy_classification（敵認定）
          → attack_justification（攻撃の正当化）
```

## 具体例：願いの政治化

```
「平和を願う」
  → 「反戦」（平和＝戦争反対）
    → 「左翼」（反戦＝左派の主張）
      → 「反日」（左翼＝反日勢力）
        → 「攻撃対象」（反日＝敵）
```

各ステップの論理的飛躍：
- 平和を願う → 反戦：妥当（だが「反戦」にはニュアンスがある）
- 反戦 → 左翼：一部の連想（反戦は左右問わず存在）
- 左翼 → 反日：論理的飛躍（左翼＝反日ではない）
- 反日 → 攻撃対象：正当化の完了

## 発動条件

1. 二項対立的な政治構造（左/右、敵/味方）
2. ラベルの負の連想（「左翼」「反日」のスティグマ）
3. 連鎖を検証しない受け手（各ステップを批判的に見ない）
4. 攻撃欲求の存在（ラベルは攻撃の口実）

## 失敗条件

- **連鎖の可視化**: 各ステップの飛躍を指摘される
- **ラベルの無効化**: ラベル自体が力を持たない文脈
- **多義性の回復**: 「反戦」が左右両方にあることの認識
- **発話者の信頼**: 「この人が反日なわけない」という認識

## 適用事例

| Layer | Entities |
|-------|----------|
| politics | red-scare, anti-national-labeling, cancel-culture |
| history | mccarthyism（共産主義者認定）, witch-hunt |
| technology | hashtag-hijacking, context-collapse |
| philosophy | guilt-by-association, slippery-slope-fallacy |

## ラベリング連鎖の類型

| 起点 | 連鎖 | 終点 |
|------|------|------|
| 平和を願う | 反戦→左翼→反日 | 攻撃対象 |
| 環境保護 | エコ→リベラル→反経済 | 攻撃対象 |
| 伝統重視 | 保守→右翼→差別主義 | 攻撃対象 |
| 効率重視 | 合理主義→冷酷→非人間的 | 攻撃対象 |

## 関連パターン

- **purity**: ラベリングは純粋性判定の手段
- **chilling-effect**: ラベリングへの恐怖が沈黙を生む
- **rationalization**: ラベリングは攻撃の合理化
- **causal-misattribution**: 連鎖は因果の誤帰属を含む
- **exit-blockade**: 逃げられない環境でラベリングが武器化

## 出典記事

`200_Output/note-articles/wish-silencing-structure.md`

## メカニズムID

**[T-045] Labeling Cascade** — ラベリング連鎖による敵認定
