# structure-decoder

**テキストを構造で読むための、辞書 × エンジン。**

書物・記事・目の前の状況を、蓄積された **atoms（構造原子）** と **patterns（構造パターン）** を通して分解・命名する。

> 「材料」ではなく「料理とレシピ」を出す。
> 一次資料は持ち込まず、抽出された構造辞書と、それを動かす分解エンジンだけを公開する。

---

## 何ができるのか（具体例）

たとえば、カフカの『変身』第1章の冒頭。グレゴールが虫になった朝、彼は虫になったことより先に出社の段取りを確認する。なぜそうなるのか？

generic LLM は「主人公の混乱を示しています」と要約する。structure-decoder はこう答える：

```
検出された atoms:
  - context-stripping（コンテキスト剥離）
  - prevention-invisibility（予防の不可視性、反転形）

起動している patterns:
  - inquiry-foreclosure（問いの先回り閉鎖）
  - sudden-obsolescence（即時的旧式化）
  - malice-threshold-lowering（悪意敷居の低下）

新造語候補:
  - 役割剥落の即時性
  - 鳴き分け（意味と原音の分離）
  - 訴権の事前消去
```

「**訴える権利は、訴えの内容が審査される前に剥奪される**」——この構造を、カフカの文学からも、現代の組織からも、同じ語彙で取り出せる。それが structure-decoder の中身です。

実物：[`examples/henshin/chapter-1-reading-note.md`](examples/henshin/chapter-1-reading-note.md)

---

## なぜ作るのか

AI が要約・翻訳を担う時代に、人間に残された仕事は「**何をやるべきかを自分で見つけ、構造として名指す**」こと。

generic な LLM は「この文章を要約して」には答える。だが「この文章にどの構造パターンが起動しているか」には答えられない。なぜなら、その**事前辞書**を持っていないから。

structure-decoder は、数百冊の読書と数百日の観察から抽出された辞書を、誰でも引けるようにする装置です。Christopher Alexander の『パタン・ランゲージ』が建築でやったことを、テキストと状況の領域で。

---

## 中身

```
structure-decoder/
├── dictionary/                # = 脳そのもの
│   ├── atoms/                # 構造原子（79件）
│   ├── patterns/             # 構造パターン（232件）
│   ├── mechanisms/           # OS層メカニズム（34件）
│   └── meta/                 # メタ層（書物レベル技法など）
├── .claude/skills/            # = 分解エンジン（Claude Code が自動読込）
│   └── book-decompose/       # 書物の一文を4層分解 + 5 modes
├── examples/                  # = 装置が動いた証拠
│   └── henshin/              # 変身（カフカ）全3章 reading-note + published
└── docs/                      # = 方法論（執筆中）
```

### 辞書の三層

| 層 | 単位 | 役割 | 件数 |
|---|---|---|---|
| **atoms** | 構造原子 | 分解不可能な最小単位の動作・関係 | 79 |
| **patterns** | 構造パターン | atom の組み合わせで生まれる再現可能な構造 | 232 |
| **mechanisms** | OS層 | パターンを跨いで作用する civilization-level の動因 | 34 |

各辞書ファイルには `derived_from`（出典）が記載されています。一次資料の本文は含めず、書名・著者・年・章のみを参照として残す方針です。

---

## 使い方

### 1. クローン

```bash
git clone https://github.com/Ujiie1101/structure-decoder.git
cd structure-decoder
```

### 2. 辞書を引く（読み物として）

```bash
# 全 atoms の一覧
ls dictionary/atoms/

# ある atom の中身を読む
cat dictionary/atoms/context-stripping.md
cat dictionary/patterns/inquiry-foreclosure.md
```

辞書ファイルはすべて Markdown + frontmatter。GitHub上でも読めます。

### 3. 装置を動かす（Claude Code で 4層分解）

このリポジトリで `claude` を起動すると、`.claude/skills/` が自動的に読み込まれ、`/book-decompose` コマンドが使えるようになります。

```bash
# このディレクトリで Claude Code を起動
claude

# 起動後、次のコマンドを実行：
/book-decompose 「親譲りの無鉄砲で小供の時から損ばかりしている」 坊っちゃん
```

出力例：4層分解（事実 / 修辞 / 構造命題 / 書物接続）+ 起動した atoms / patterns のリスト + 新造語候補。

その他のモード：

```
/book-decompose --extract <段落>           # load-bearing 文の抽出
/book-decompose --article <文>             # 古典×現代の記事執筆
/book-decompose --en <文>                  # 英訳版（海外ブログ用）
/book-decompose --reading-note <章>        # 観察者の独白（内部用）
/book-decompose --published <章>           # note 公開用 ※注釈形式
```

> **Note**: Claude Code（Anthropic公式CLI）が必要です。インストールは `npm install -g @anthropic-ai/claude-code` または公式手順（[docs.anthropic.com/claude/docs/claude-code](https://docs.anthropic.com/claude/docs/claude-code)）を参照してください。Anthropic API キーまたは Claude Pro/Max 等の対応プランが必要です。

---

## ステータス

**WIP — v0.4（dictionary + 3 engines + 3 サンプルセット + methodology 公開）**

| フェーズ | 進捗 |
|---|---|
| dictionary 層 | ✅ atoms 79 / patterns 232 / mechanisms 34 / meta 3 |
| engines 層 | ✅ `book-decompose` / `atom-decompose` / `diagnose`（3エンジン、3入力チャネル全稼働） |
| examples 層 | ✅ 変身（カフカ）/ 坊っちゃん（漱石）/ 斜陽（太宰） 合計22章（reading-note + published） |
| docs/methodology | ✅ [docs/methodology.md](docs/methodology.md) |
| 図解 / デモ | ⏳ Mermaid 図 + asciinema cast 予定 |
| CONTRIBUTING / Issue templates | ⏳ 予定 |
| Web UI | ⏳ 将来 |

移植元: 非公開の個人作業vault（数百冊の読書と数百日の daily-writing から構築）

詳しい方法論は [`docs/methodology.md`](docs/methodology.md) を参照。4層分解の原理、辞書の三層構造、エンジンの動作、新規 atom/pattern の追加方法まで。

---

## ライセンス

MIT License — 商用利用・改変・再配布いずれも自由です。`derived_from` の出典は維持してください（学術的誠実性のため）。
