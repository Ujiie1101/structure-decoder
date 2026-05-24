# Contributing to structure-decoder

このリポジトリは「テキスト・状況を構造で読む装置」です。貢献は **辞書（dictionary/）の拡張** と **エンジン（.claude/skills/）の改良** が中心です。

**先に読むべき文書**：[docs/methodology.md](docs/methodology.md) §6「拡張方法」。本 CONTRIBUTING.md は、その上に乗る GitHub ワークフロー上の運用ルールを補足します。

---

## 1. 何を welcome / 何を welcome しないか

### Welcome

- 新しい **atom**（構造原子）の提案 — 既存 79 件と独立で、3 場面以上で観察されたもの
- 新しい **pattern**（構造パターン）の提案 — 既存 atom の組み合わせとして公式化できるもの
- 新しい **example**（書物・記事・状況の分解結果） — 既存辞書を使った実演
- 既存 atom / pattern の **反証事例** — 「この atom が成立しない事例」も価値あるデータ
- ドキュメント改善・誤字修正・リンク切れ
- エンジン skill の挙動改善・バグ修正

### Welcome しない

- ❌ **既存 atom / pattern のリネーム**だけの PR（理由なき改名は破壊的変更）
- ❌ **印象批評・要約・感想**を `examples/` に追加する PR（4 層分解の形式を取らないもの）
- ❌ **出典 (`derived_from`) のない** atom / pattern 追加
- ❌ **独立性チェックを通っていない** atom 追加（既存 atom に包含される構造）
- ❌ 一次資料の本文を含める PR（書名・著者・年・章のみが方針）

---

## 2. 開始する前に

### 必須の事前準備

1. [README.md](README.md) を読む — 何を作っているか
2. [docs/methodology.md](docs/methodology.md) を読む — なぜこの形か、4 層分解の原理、辞書三層、再現性の定義
3. 関連する既存 atom / pattern を **5 件以上読む** — 命名規則・粒度感・frontmatter 形式を体感する

### Issue を先に立てるべきケース

- 新規 atom / pattern の提案（マージ前に独立性・粒度を議論したい）
- 既存 atom / pattern の **大幅改訂**（破壊的変更）
- エンジン skill の挙動を変える提案

小さな修正（誤字、リンク切れ、観察事例の追加）は直接 PR で OK。

---

## 3. 種類別 PR ガイド

### 3-1. 新しい atom を追加する

**条件**（methodology §6 から再掲）：

1. これ以上分解すると構造が消えることが確認できる
2. **3 つ以上の異なる場面**で再現観察されている
3. 既存 atom に包含されない（独立性チェック済み）

**手順**：

```bash
# 1. ブランチを切る
git checkout -b atom/your-atom-id

# 2. ファイル作成
touch dictionary/atoms/your-atom-id.md

# 3. テンプレートに沿って記述（→ methodology §6）

# 4. _index.md を更新（atom 一覧に追加）
edit dictionary/atoms/_index.md

# 5. 関連する既存 atom / pattern の "関連" セクションに双方向リンクを追加
```

**PR 本文に必須の項目**：

- 観察事例 3 件以上（出典付き）
- 独立性チェック：「この atom は既存の {X} とは違う、なぜなら …」を明示
- 既存 pattern に再分解する場合、composition の更新案

### 3-2. 新しい pattern を追加する

**条件**：

1. 複数の atom が組み合わさって**再現可能な複合構造**が見える
2. 構成 atom が `dictionary/atoms/` にすでに存在する（先に atom 追加）
3. **反証条件**を最低 3 つ書ける

**手順**：

```bash
git checkout -b pattern/your-pattern-id
touch dictionary/patterns/your-pattern-id.md
# テンプレ → methodology §6
# composition_formula で構成を明示
```

**PR 本文に必須の項目**：

- 適用事例：最低 3 ドメイン横断
- 反証条件：パターンが成立しない条件
- 関連 pattern との差分（似ているが独立である根拠）

### 3-3. 新しい example を追加する

`examples/{book-name}/` を新規作成し、`/book-decompose --reading-note` や `--published` の出力を配置します。

**形式の選択**：

| Mode | ファイル名 | 文体 | 用途 |
|---|---|---|---|
| Mode 5 | `chapter-N-reading-note.md` | だ・である調 | 観察者の独白（内部分析） |
| Mode 6 | `published/chapter-N.md` | ですます調・※注釈形式 | note / blog 公開向け |

**条件**：

- 4 層分解の形式を取っていること（事実 / 修辞 / 構造命題 / 接続）
- 起動した atoms / patterns を frontmatter の `kos_internal_refs` に明示
- 一次資料は引用最小限（**書名・著者・年・章のみ**を残す）

### 3-4. バグ修正 / 誤字 / リンク切れ

issue 不要、直接 PR で OK。1 PR = 1 修正の方針。

---

## 4. PR チェックリスト

PR を出す前に確認：

- [ ] frontmatter が既存 atom / pattern と同じ形式
- [ ] `derived_from` または出典情報がある（atom / pattern の場合）
- [ ] 独立性チェックを PR 本文で説明している（新規 atom / pattern の場合）
- [ ] 3 場面以上の観察事例が PR 本文または本文ファイルにある
- [ ] 関連する既存 atom / pattern に双方向リンク追加済み
- [ ] `_index.md` を更新済み（該当する場合）
- [ ] 一次資料の本文を含めていない

---

## 5. レビュー基準

PR は以下の軸でレビューされます：

| 軸 | 質問 |
|---|---|
| **独立性** | 既存 atom / pattern に包含されないか？ |
| **再現性** | 別の読み手が同じ判定に到達できるか？ |
| **反証可能性** | 「この atom / pattern が成立しない条件」を書けるか？ |
| **粒度の一貫性** | 既存辞書の粒度感と揃っているか？ |
| **命名の正確性** | 名前が動作・関係を捉えているか？「現象」「結果」になっていないか？ |

**フィードバックの形**：構造的にズレている場合は具体的に指摘します。お世辞は言いません。**「マージしない」も明確に伝えます**（人格批判ではなく、辞書の一貫性のため）。

---

## 6. レビュープロセス

- 初回レスポンス目標：**7 日以内**
- マージ判断：辞書の一貫性を優先するため、急ぎません
- 大きな PR は **段階的にマージ**することがあります（atom だけ先、pattern は議論継続など）

---

## 7. コミュニケーション

- 議論は **GitHub Issue / PR コメント** で
- 質問のための Issue も welcome（`question` ラベル）
- 既存 atom / pattern への異議申し立ても welcome（`challenge` ラベル）

---

## 8. ライセンスと帰属

- リポジトリのライセンスは **MIT**。貢献内容も MIT で受け入れます
- 各 atom / pattern の `derived_from` は **必ず維持**してください（学術的誠実性のため）
- 大きな貢献者は将来 `CONTRIBUTORS.md` を作成して記載予定

---

## 9. 行動規範

知的誠実さ、構造的議論、相手の貢献への敬意を基本とします。**「あなたの読みは違う」と「あなたは間違っている」を分けて議論できる**人を歓迎します。

ハラスメント、差別的発言、人格攻撃は理由を問わず排除します。

---

> 一冊の本、一つの状況、一つの観察が、辞書を 1 件分前に進めます。
> あなたの読みを、構造として共有してください。
