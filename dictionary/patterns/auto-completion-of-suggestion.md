---
id: "auto-completion-of-suggestion"
name: "暗示の自己完成"
grammar_type: "transformation"
created: 2026-05-13
source_work: "夏目漱石『坊っちゃん』第六章（舟上で暗示を浴びた坊っちゃんが一晩寝た翌朝『山嵐は裏切り者』と確信している）"
composition:
  - atom: adjective-arrow
    role: 形容詞だけが投下される
  - atom: narrative-pressure
    role: 受け手が物語化可能な命題を補完する
---

# auto-completion-of-suggestion（暗示の自己完成）

撒かれた暗示が、**受け手の中で時間をかけて固有名と結びつき、命題として自己完成する**過程。撒いた本人はもうそこにいない。受け手は完成した命題を「自分が思いついたもの」として抱える。

## 定義

時系列構造:

1. **撒火**: 攻撃者Aが形容詞・断片だけを発する
2. **休眠**: 受け手Bは一定時間（数時間〜数日）保持する
3. **発芽**: B自身の記憶・推論によって固有名Cが補完される
4. **自己所有**: Bは「私が考えた」と命題を所有する
5. **行動**: BはCに対して敵対的行動を取る

攻撃者Aは後で問い詰められても「私はそんなことは言っていない」と答えられる。実際、Aが発した言葉は形容詞だけだった。

## 構造

```
suggestion_drop（暗示投下）
  → temporal_dormancy（休眠）
    → memory_consolidation（記憶統合過程で命題化）
      → self_attribution（自分の判断と認知）
        → autonomous_action（命題に基づく行動）
```

睡眠・休憩・通勤などの非意識的処理時間が、自己完成を加速する。

## 観察可能な現代具体例

- 上司との会話の翌朝、特定の同僚への評価が変わっている
- 一晩寝たら「あの人は危険」と確信が固まっている
- 「自分の意見」だと思っていることが、実は誰かに昨日撒かれた種だった
- アルゴリズム推薦経由のニュース消費後、自然と特定の政治観に着地する

## 対抗装置

- [second-information-axis](../atoms/second-information-axis.md) — 別情報源との照合
- 「この命題を最初に聞いたのは誰か」と発生源を遡る習慣
- 翌朝の確信を一日待つ（休眠による発芽を可視化する）

## 関連パターン

- [un-accusable-attack](un-accusable-attack.md) — 上位メタパターン
- [labeling-cascade](labeling-cascade.md) — 連想による自己強化との類似
- [innuendo-broadcast](innuendo-broadcast.md) — 撒火の場面装置
