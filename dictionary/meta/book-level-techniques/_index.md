---
type: index
subtype: book-level-techniques
created: 2026-05-13
status: prototype-v0.1
---

# Book-Level Techniques — 書物全体に効く操作技法

## 目的

通常の `130_Structure/atoms/` は **event-level**（事象内部の動作原子）を扱う。
本サブディレクトリは、それより上位のスケール、**book-level**（書物・物語・運動の全体テキスト構造に効く操作技法）を扱う。

```
事象内部の動作 → atoms/ (event-level)
   ↓
事象の集まり方 → patterns/ (event-level)
   ↓
書物全体の構造 → book-level-techniques/ (book-level) ← ここ
```

## なぜ別レイヤーか

event-level atoms との違い:

| 観点 | event-level atom | book-level technique |
|---|---|---|
| 操作対象 | 事象内部の動作 | テキスト全体・書物全体 |
| 効く時間 | 事象同時 | 事後（読者の認知の中）|
| 担い手 | 当事者 | 書き手（編集権力）|
| 一語の重み | 並列の構成要素 | 書物全体を再定義する錨 |

通常atomは「事象を分解した動作」、book-level techniqueは「事象群を編集する書き手側の技法」。両者は別レイヤーで併存する。

## ファイル構造

各 technique ファイル（`{id}.md`）の必須セクション:

```yaml
---
id: "..."
name: "..."
type: "meta-atom"
scope: "book-level"
domain: "literary-architecture"
created: ...
source_work: "..."
related_atoms: [event-level atom ids]
related_patterns: [pattern ids]
---

# {name}

1段落の定義。

## 起源（Why this exists）
なぜ書物・物語にこの技法が現れるか。

## 観察可能なproxy
発動を検知する具体的シグナル（書物・組織・物語・運動における）。

## 通常atomとの違い（event-level vs book-level）
階層上の位置と効き方の差。

## 介入点／応用可能性
書字者として運用するときの判断、読者として見抜くときの観点。

## 関連technique
他のbook-level techniqueとの関係、関連atom/pattern。

## 出典書物における運用（任意）
発見元の書物での具体的運用パターン。
```

## 登録状況

### v0.1（2026-05-13）— 太宰治『斜陽』由来

| Technique | Source | Domain |
|---|---|---|
| [chapter-pivot-line](chapter-pivot-line.md) | 斜陽全八章末尾の一行 | literary-architecture |
| [title-self-inversion](title-self-inversion.md) | 斜陽→太陽の書名反転 | literary-architecture |

book-series skill による book-decompose 方法論の副産物。`.neologism-buffer.json` で `atom-candidate-meta` / `atom-candidate-book-level` とタグ付けされていた候補2件を本層に正式登録。

## 次の拡張候補

- `omnibus-summoning`（複数章を1記事に再縫合する技法 / 坊っちゃん omnibus 由来）
- `mirror-chapter-pairing`（第N章と第N'章を鏡像配置する技法 / 斜陽第4章＝第7章対称由来）
- `sign-cascade-trigger`（冒頭徴候の連鎖発火 / 斜陽の蛇→母の死→書名反転の系列由来）

これらは今後の book-series 運用で別書物から候補が出てきた時に正式提案する。

## 関連レイヤー

- [130_Structure/atoms/](../../130_Structure/atoms/) — event-level の構成要素プリミティブ
- [130_Structure/patterns/](../../130_Structure/patterns/) — event-level の中粒度構造
- [`.claude/skills/book-decompose/`](../../../.claude/skills/book-decompose/) — book-level 操作を生成する skill
- [`.claude/skills/book-series/`](../../../.claude/skills/book-series/) — book-level 操作を連載化する skill
