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
├── engines/                   # = 分解エンジン（Claude Code skills、移植中）
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

## 使い方（v0、現状）

このリポジトリを clone し、`dictionary/atoms/` `dictionary/patterns/` を辞書として参照します。

```bash
git clone https://github.com/Ujiie1101/structure-decoder.git
cd structure-decoder
# atoms/patterns を読んで構造のレキシコンを得る
ls dictionary/atoms/
ls dictionary/patterns/
```

実行可能なエンジン（Claude Code skills）の移植は近日中に `engines/` に追加します。最終的には：

- Claude Code から `/book-decompose` 等のコマンドで分解実行
- もしくは Web app から paste して分解実行

---

## ステータス

**WIP — v0.1（dictionary + 1サンプルセット 公開）**

| フェーズ | 進捗 |
|---|---|
| dictionary 層公開 | ✅ atoms 79 / patterns 232 / mechanisms 34 / meta 3 |
| examples 層公開 | ✅ 変身（カフカ）全3章 |
| engines 層公開 | ⏳ Claude Code skills 移植中 |
| docs/methodology | ⏳ 執筆中 |
| Web UI | ⏳ 将来 |

移植元: 非公開の個人作業vault（数百冊の読書と数百日の daily-writing から構築）

---

## ライセンス

MIT License — 商用利用・改変・再配布いずれも自由です。`derived_from` の出典は維持してください（学術的誠実性のため）。
