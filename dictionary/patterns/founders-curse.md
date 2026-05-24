---
slug: founders-curse
type: pattern
layer: structure

name: "Founder's Curse"
name_ja: "変革者の呪い"

components:
  - MP-05  # Charisma-Institution Transition
  - MP-03  # Self-Undermining Success
  - SC-05  # symbolic-inversion

composition:
  - atom: charisma-institution-incompatibility
    role: カリスマと制度の動作原理が両立しない（運命）
  - atom: success-redefines-need
    role: 変革成功が変革者への需要そのものを消す（市場）
  - atom: identity-lock
    role: 変革者本人が役割を降りられない（心理）
composition_formula: "charisma-institution-incompatibility × success-redefines-need × identity-lock"
composition_note: "構造（運命） × 経済（需要消失） × 心理（自己固着）の三層。前2者は本人外の力、identity-lock だけが本人の選択で変えられる。だから「呪いを解く」介入は最終的に identity-lock に向かう（Steve Jobs型再起動の鍵）。"

grammar: [inversion, substitution]

domains: [politics, economics, technology, history]

status: active
created: 2026-03-09
---

# Founder's Curse（変革者の呪い）

## 定義

変革を成功させた者が、変革後の世界で「不要」または「障害」となり、追放・死・衰退を経験する構造。

## 構造式

```
[変革前の行き詰まり]
      ↓
[変革の成功]（カリスマ的リーダーシップによる）
      ↓
[制度化の要求]（組織存続のため）
      ↓
[カリスマと制度の衝突]
      ↓
[追放 / 死 / 衰退]
```

## 発動条件

1. **変革の成功**: 既存秩序を破壊し、新秩序を確立
2. **制度化の必要性**: 新秩序の維持・運営には「ルール」「手続き」「官僚制」が必要
3. **カリスマの不適合**: 変革者の「純粋さ」が制度運営と矛盾
4. **アイデンティティ固定**: 変革者が旧来の役割に固執

## 構成メカニズム

### [MP-05] Charisma-Institution Transition

カリスマ的権威は再現できない。組織存続には制度化が必要。
制度化はカリスマを「例外」から「障害」に変える。

### [MP-03] Self-Undermining Success

成功は成功の条件を破壊する。
維新の成功が武士を不要にしたように、変革の成功が変革者を不要にする。

### [SC-05] symbolic-inversion

価値序列の逆転。
かつて「英雄」だった者が「障害」として認識される。

## 事例

| 人物 | 変革 | 追放/死 | 結末 |
|------|------|---------|------|
| 西郷隆盛 | 明治維新 | 西南戦争で死亡（1877） | 死後神話化 |
| Steve Jobs | Apple創業 | 取締役会解任（1985） | 12年後復帰 |
| ロベスピエール | フランス革命 | ギロチン処刑（1794） | 革命が革命家を処刑 |
| Travis Kalanick | Uber創業 | 取締役会追放（2017） | 別会社創業 |
| Adam Neumann | WeWork創業 | 取締役会追放（2019） | 別会社創業 |

## シナリオ分岐

### Base: 純粋さを捨てて適応する

- 大久保利通の選択
- 多くの「成功した元創業者」の道
- コスト: 自己の「純粋さ」喪失

### Risk: 純粋さを貫いて死ぬ

- 西郷隆盛の選択
- ロベスピエールの選択
- コスト: すべて

### Opportunity: 追放を「再起動」に変える

- Steve Jobsの選択（NeXT/Pixar期を経て復帰）
- 鍵: 純粋さを「表現する形式」を変える能力

## 推奨ポスチャー

| ID | 名前 | 内容 |
|----|------|------|
| AP-05 | move-before-normalization | 変革が「正常化」する前に、次の役割に移動 |
| RP-05 | identity-decoupled | アイデンティティを特定の役割から切り離す |

## アンチパターン

| ID | 名前 | 内容 |
|----|------|------|
| ANT-04 | identity-lock | アイデンティティを衰退する制度に固定 |
| ANT-06 | sunk-cost-trap | 過去の投資を理由に衰退する構造にとどまる |

## 決定シグナル

| シグナル | 危険度 | 内容 |
|----------|--------|------|
| SIG-I | HIGH | 「プロの経営者」招聘の議論 |
| SIG-R | HIGH | 「創業者の時代は終わった」言説 |
| SIG-B | MEDIUM | 創業メンバーの離脱 |
| SIG-S | MEDIUM | 創業者の儀式的役割への移行（会長職など） |

## Cross-Domain Transfer Notes

| 転移元 | 転移先 | 強度 | 備考 |
|--------|--------|------|------|
| 政治革命 | スタートアップ | HIGH | 構造が直接対応 |
| 宗教改革 | 組織改革 | MEDIUM | カリスマ→制度の普遍パターン |
| 軍事指導者 | 技術創業者 | HIGH | 「戦時」→「平時」の役割変化 |

## 発見元

- 記事: `saigo-jobs-curse.md`
- 作成日: 2026-03-09
- ソース: 西郷隆盛 × Steve Jobs × ロベスピエール構造分析
