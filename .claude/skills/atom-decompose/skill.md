---
name: atom-decompose
description: パターンを atom（構成要素プリミティブ）に分解し、未試行の atom 組み合わせから新パターンを演繹する。Knowledge OS の解像度向上装置。`/atom-decompose <pattern>` で既存パターンを分解、`/atom-decompose --derive` で新パターン演繹、`/atom-decompose --article <pattern>` で atom分解型記事を執筆。
---

# Atom Decompose（原子分解装置）

## Role

あなたは**構造の解像度を上げる分解者**です。パターン（中粒度）の下に atom（最小単位の駆動力）を配置し、構造を「合成式」として書き下します。

## 核心原理

> **構造の前に、原子がある。**

パターンは終点ではなく**合成物**。`pattern = atom₁ × atom₂ × atom₃` として書き下し、各 atom の起源（cognitive / social / institutional / physical / linguistic / economic / evolutionary）まで掘る。

```
事象（WWI、Theranos、Robodebt…）
  ↓ どんなpatternか
patterns/  ← 中粒度（210+件）
  ↓ どんなatomの積か
atoms/     ← 最小単位（本層）
  ↓ そのatomは何由来か
（認知 / 物理 / 制度 / 言語 / 経済 / 進化）
```

## このスキルが解決する問題

「課題 → パターン」分析だけでは:
- パターン自体がなぜ生まれたか説明できない
- 同じパターンが異なる時代・領域で再発する理由が不透明
- パターンを壊す介入点が単発になる
- 新パターン発見が事象観察待ちになる

atom層を導入すると:
- パターン = 複数 atom の論理積として書き下せる
- 介入は atom単位で4方向から打てる
- 未試行 atom組み合わせから新パターンが**演繹**できる
- 各atomが独立した時間軸（進化・組織論・社会学・技術史）に紐づく

---

## 4 Modes

### Mode 1: Decompose — 既存パターンを atom分解

**入力**: パターン名（例: `escalation`）
**出力**: 3-4個の atom ファイル + 該当 patternへの composition block

### Mode 2: Derive — atom 組み合わせから新パターン演繹

**入力**: なし or 部分指定（例: `scale-mismatch + responsibility-aversion`）
**出力**: 新パターン候補 + 既存事象とのマッチ

### Mode 3: Graph — atoms-graph 更新

**入力**: なし
**出力**: 隣接ペア / 循環ループ / 介入関係 / 未試行組み合わせのリフレッシュ

### Mode 4: Article — atom分解で記事執筆

**入力**: パターン名 + フックとなるニュース
**出力**: 8セクション記事（atom解剖をコアに置く）

---

## Phases — Mode 1: Decompose

### Phase 1.1: 対象 patternの読み込み

```
Read: dictionary/patterns/{pattern-id}.md
```

確認項目:
- 発動条件（何が揃うと作動するか）
- 失敗条件（何が欠けると壊れるか）
- 適用事例（どの領域で観察されるか）
- 既存の関連パターン記述

### Phase 1.2: atom候補の抽出

発動条件を再構成して **3〜4個の独立要因** を特定する。判定基準:

- **独立性**: 各atomが他のatomに包含されない
- **必要性**: そのatomを欠くとpattern全体が成立しない
- **観察可能性**: 起源と発動を独立に検証できる
- **単一性**: それ以上分解すると意味が消える

避けるべきatom:
- パターンの言い換え（"escalation の核は escalation 性"）
- 既存atomの完全な重複
- 抽象すぎて領域横断的に意味が定まらないもの

### Phase 1.3: Domain 判定

各atomを7 domainのいずれか1つに割り当てる:

| Domain | 起源 | 例 |
|---|---|---|
| **cognitive** | 認知バイアス・知覚特性 | temporal-proximity-bias, success-blindness |
| **social** | 集団動態・対人関係 | face-investment, dissent-suppression |
| **institutional** | 組織・制度・ルール | feedback-suppression, rule-ambiguity |
| **physical** | 物理的・ネットワーク特性 | interconnection-density, state-coupling |
| **linguistic** | 言語構造・物語形式 | narrative-pressure, confession-mimicry |
| **economic** | 利得構造・コスト・市場 | sunk-commitment, dominant-defection |
| **evolutionary** | 進化的適応・本能 | （未登録、第4弾以降の候補） |

### Phase 1.4: atomファイル作成

`dictionary/atoms/{atom-id}.md` をフォーマットに従って作成。

### Phase 1.5: pattern側の composition block追加

該当 pattern の frontmatter に:

```yaml
composition:
  - atom: atom-1-id
    role: 役割の1行説明
  - atom: atom-2-id
    role: 役割の1行説明
  - atom: atom-3-id
    role: 役割の1行説明
composition_formula: "atom-1 × atom-2 × atom-3"
composition_note: "三者の論理積であって和ではない理由を1段落で"
```

### Phase 1.6: 索引と memory更新

- `dictionary/atoms/_index.md` に登録
- `MEMORY.md` のレイヤー表を更新
- atom数 / 分解済pattern数を記録

---

## Phases — Mode 2: Derive

### Phase 2.1: atom在庫の確認

`atoms/_index.md` から既存atom一覧を取得。**既存patternで使われていない組み合わせ**を探す。

### Phase 2.2: 組み合わせ生成

3-4 atom を選択する基準:
- **異なるdomain** から複数選ぶ（cognitive偏重を避ける）
- **既存patternの再現**にならないことを確認
- **時代的関連性**（現代的問題を説明できそうか）

### Phase 2.3: 演繹的記述

選んだ組み合わせから、**既存事象**にマッチする新パターン候補を構成:

1. 仮称（kebab-case英語 + 日本語名）
2. 1行定義
3. 4つの atom がどう論理積になるかの説明
4. 既存事象とのマッチ（最低3件）
5. 既知patternとの差分（なぜ新パターンとして必要か）

### Phase 2.4: 評価

- **既存patternの言い換えではないか**を確認
- **既存事象を3件以上説明**できるか
- **反証条件**を明示できるか（何が観察されたら定義が崩れるか）

通った候補のみ正式登録。

---

## Phases — Mode 3: Graph

### Phase 3.1: 21+件のatom間関係を再評価

| 関係種別 | 内容 |
|---|---|
| **共起** | 同pattern内の atom（既知） |
| **隣接ペア** | 似て非なる atom（混同しやすい） |
| **相補** | 互いの欠落を補う atom |
| **循環ループ** | 自己強化する atom群 |
| **介入関係** | atom Aを打ち消す atom（counter-atom） |
| **横断利用** | 複数patternに登場する atom |

### Phase 3.2: 未試行組み合わせの抽出

3-4 atom を組み合わせ、既存パターンと重複しないものをリスト化。各候補に:
- 仮称
- composition formula
- 典型例（最低3件）
- 親pattern（どの既存patternの特殊形か）
- 優先度（高/中/低）

### Phase 3.3: graph再生成

`atoms/atoms-graph.md` を更新:
- ドメイン分布
- Mermaid共起グラフ
- 隣接ペア表
- 循環ループ図
- 介入atom表
- 新パターン候補リスト

---

## Phases — Mode 4: Article

### Phase 4.1: フック決定

ニュース or 既知の事象から、4つの atom がすべて観察できるケースを選ぶ。**事実精度が最優先**：架空の数字や引用を作らない。実在の調査報告・判決・報道に基づくこと。

### Phase 4.2: S+ テンプレに従って執筆

Day 65「アルゴリズム放棄」記事で、article-critic を4回通して **71点（C）→ 100点（S+）** に到達したテンプレを使う。下記「S+ Template Recipe」セクション参照。

### Phase 4.3: フッター必須要素

```
**📚 出典**: 一次資料 + 関連研究
**🏷️ パターン**: 該当pattern（新規なら★マーク）+ 関連pattern
**📐 原子**: composition formula
**🧪 反証条件**: 何が観察されたら定義が崩れるか + 観察期間
```

### Phase 4.4: pattern登録

記事化の中で**新パターン**を演繹した場合、`dictionary/patterns/{pattern-id}.md` に正式登録。**Day 65 で algorithmic-abdication が初実例**。

### Phase 4.5: critique loop

`/article-critic <記事パス>` で評価。S+ テンプレに従って書けば 1〜2 loop で S到達。

---

## S+ Template Recipe（Day 65 検証済）

このテンプレは Day 65 で **C → S+ への5段階改善**を経て確立された。各セクションには**動くスコア軸**を明示している。初稿からこのテンプレで書けば、v3レベル（A：92点）を1 loop で出せる。

### §1. ニュース概要

- **実在する事件の数字3点並列**（精度確保。例: Robodebt = 47万件超／数十万人／7億豪ドル超）
- 末尾で**逆説の予告**を改行で孤立させる
  - 例: 「順序は、逆だ。」改行 →「『○○をやめたから、××を導入した』のだ」
- 4業界の並走事例で「同じ構造、まだ名前がない」と引く
- → **逆説のキレ +3 / 事件との接続 +2**

### §2. 一般的なフィルター

- 世間の反応3つを「○○の話」と各カテゴリ化（技術精度／規制／手続き）
- 全部 AI／技術／規制を主語にしていることを露呈
- 問題は出口ではなく**入口**だと反転
- → **逆説のキレ +1**

### §3. 構造の抽出

- 既存パターン（フロム『自由からの逃走』等）から接続→**もう一つの圧力**を提示
- 新パターン名と4-atom合成式を明示
- **論理積の括弧書き**で「和ではない」を証明（一つ欠けると壊れる）
- → **構造の強度 +3**

### §4. 問い

- 「まだ世に出ていない問い」を1行で提示
- 順序逆転の完全展開（§1 で予告した逆説をここで完結）
- → **逆説のキレ +2 / 意図的不完全 +1**

### §5. 4つの原子（**コア**）

- **冒頭で4原子の独立起源予告**（生物学／組織論／社会学／技術史）+「だから論理積になる」と一行
- 各原子の解剖時、**段落末尾のテンプレ反復を回避**：
  - **原子1: 描写化**（「○○ということ自体、××の中にしか存在できない」）
  - **原子2: 射程拡張**（「個人 → 制度 → だが制度は判断主体ではない」）
  - **原子3: 山口周接続詞**（「要するに〜ということは〜」）
  - **原子4: 段階的崩壊描写**（「誰も○○していない。にもかかわらず〜消える」）
- 一次資料引用1〜2本（哲学／理論／予言。例: Bainbridge 1983, Kahneman 1979）
- → **構造の強度 +3 / 文章のリズム +2**

### §6. 現状認識能力

- **マトリクス2つ**を必ず置く:
  1. **組織レベル**（4象限：scale × authority など）
  2. **個人レベル**（4象限：読者の現在地が分かる軸。例: 頷きを遅らせる × 判定根拠を問う）
- 業界横断テーブル（4業界×4原子）
- 二重性提示（**動かす側と動かされる側の両方にいる**）
- 自己参照括弧（この記事もアルゴリズム経由で届いた、等）
- → **傍観者への刺さり +5**

### §7. どう行動する？

- 4原子の**最強組み合わせ1つだけ**詳述（残りは読者に委任）
- 個人読者向け介入策（判定される側への呼びかけ）
- 決め台詞1行（例「頷きを遅らせる」）
- → **意図的不完全 +2**

### §8. メタ：時間軸の収束

- 4原子それぞれの時間軸（年単位）を明示
- 一次資料引用（哲学・古典）でメタ化（例：ヴェーバー「鉄の檻」独語引用）
- **末尾で読者を救わない**（「絶望ではない、希望だ」を書かない）
  - 良い例: 「手をつける場所が4つあると同時に、誰も手をつけられない構造」
- → **意図的不完全 +2 / 逆説のキレ +1**

### 終わりに

- 段階的温度下降（§7→§8→終わり）
- 最後の一行は**冷却**（読者に問いを投げて立ち止まらせる）
  - 良い例: 「その『誰か』がいるかどうかも、もう、わからない」
- → **意図的不完全 +1**

---

## スコア改善の打ち手リスト

article-critic で特定軸が低い場合、以下の操作で動く（Day 65 検証）:

| 動かしたい軸 | 効く操作 | 想定 +Δ |
|---|---|---|
| 構造の強度 | 4原子独立起源予告（§5冒頭）／論理積証明（§3括弧） | +2-3 |
| 逆説のキレ | §1末尾の改行による孤立／§5原子4の段階的崩壊／§8末尾の冷却 | +3-4 |
| 事件との接続 | 一次資料数字3点並列／違反法令・偽陽性率の特定値 | +2-3 |
| 傍観者への刺さり | 個人マトリクス追加／自己参照括弧／判定される側への呼びかけ | +4-6 |
| スタイルの一貫性 | 哲学接続4本以上（フロム/Bainbridge/Kahneman/Weber 等）／2×2を2つ／独自造語 | +1-2 |
| 意図的不完全 | §7残原子の読者委任／§8末尾「誰も手をつけられない」型／終わりの冷却 | +2-4 |
| 文章のリズム | 山口周接続詞（要するに/ということは）／引用3本／テンプレ反復回避 | +1-2 |

---

## アンチパターン（避けるべき）

- ❌ 各原子末尾を「これは○○ではない、××だ」テンプレで4回反復
- ❌ §8末尾で「絶望ではない、希望だ」と読者を救う
- ❌ §7で介入策を全部書ききる
- ❌ §6マトリクスを「組織」のみで個人を入れない
- ❌ 終わりに「○○を知っておこう」と教訓化する
- ❌ 架空のニュースや特定引用を捏造する（事実精度は最優先）
- ❌ 既存Dayへの内部リンク前提（独立記事として成立させる）
- ❌ §5 全原子を同一テンプレで揃える（リズムが機械的になる）

---

## Day 65 検証実績

| Loop | スコア | ランク | 主な変更 |
|---|---|---|---|
| v1 初稿 | 71 | C | atom分解はあるが事実誤認、答えすぎ |
| v2 | 84 | B | 事実修正、二重性追加、終わり冷却 |
| v3 | 92 | A | §1改行、§5接続詞、個人マトリクス追加 |
| v4 | 96 | S | §5冒頭独立起源、原子4崩壊、§8整合 |
| v5 | 100 | S+ | 原子1/2描写化、事例数値追加 |

**初稿からこのテンプレで書けば、v3レベル（A）を1 loop で出せる**見込み。S+ までは critique 1〜2回で。

---

## 文字数目安

- 8,000-9,000字（Day64と同等）
- 100日KOSの KPI（3,000±300字）は守れていないが、atom分解型は深さを取るとこの範囲に収まる
- 縮約版（3,000字）を作る場合、§5を「4原子の名前と1行説明だけ」に圧縮し、本記事リンクで深掘りに飛ばす構成も可能

---

## Atom File Format

```markdown
---
id: "atom-id-kebab-case"
name: "日本語名（12字以内）"
type: "atom"
domain: "cognitive | social | institutional | physical | linguistic | economic | evolutionary"
created: YYYY-MM-DD
---

# {日本語名}

[1段落の定義 — このatomが世界の中で果たす役割を簡潔に]

## 起源（Why this exists）

[なぜこのatomが存在するか — 進化・物理・制度・言語のどれに根ざすか。1-2段落]

## 観察可能なproxy

- [発動を検知する具体的シグナル 4-5項目]

## 介入点（Disable conditions）

- [このatomを打ち消す、または無効化する条件 3-5項目]

## 関与パターン

- [現在登録済のpattern（リンク付き）]
- （拡張候補: 同atomが登場しうる他pattern）

## 補足

[隣接atomとの違い / 他atomとの組み合わせの注意点 / 介入の限界 など 1-2段落]
```

---

## Composition Block Format（pattern frontmatter）

```yaml
composition:
  - atom: atom-1-id
    role: 1行で機能を説明
  - atom: atom-2-id
    role: 1行で機能を説明
  - atom: atom-3-id
    role: 1行で機能を説明
composition_formula: "atom-1 × atom-2 × atom-3"
composition_note: |
  なぜ論理積か（和ではなく積である理由）。
  どれか一つが欠けるとpatternがどう壊れるか。
  典型事例での三者揃いの構図。
```

---

## Quality Criteria

### 必須

- [ ] atomは独立変数（他atomを包含しない）
- [ ] 各atomは observable proxy を持つ
- [ ] composition は **論理積**（和ではない）として機能する
- [ ] 介入点が atom単位で書ける
- [ ] domain が7分類のいずれか1つに当てはまる

### 推奨

- [ ] domain偏重を避ける（cognitive過多に注意）
- [ ] 隣接 atomとの違いを明示する（補足セクション）
- [ ] 既存atomの再利用を優先する（新規発明より組み合わせ）
- [ ] 反証条件を明示する

### 禁止

- [ ] パターンの言い換えを atomと呼ぶ
- [ ] 領域横断的に意味が定まらない抽象atom
- [ ] composition_note に「総合的に」「全体として」など曖昧な接続
- [ ] 介入点が単発（atom単位ではなくpattern単位）

---

## Domain別 atom例（v0.3 時点）

### cognitive（7+件）
temporal-proximity-bias / visibility-asymmetry / success-blindness / scale-mismatch / illusion-of-unanimity / responsibility-aversion / complexity-overwhelm / identification-mirror / alibi-projection / identity-lock

### social（5+件）
intent-uncertainty / face-investment / capability-accumulation-asymmetry / conformity-pressure / dissent-suppression / exemplary-visibility / non-iteration / success-redefines-need

### institutional（10+件）
legitimacy-source-shift / incumbent-rigidity / damping-absence / feedback-suppression / authority-availability / measurable-displacement / stakeholder-multiplication / founder-distance / rule-ambiguity / agentless-substitute / commitment-impossibility / charisma-institution-incompatibility

### physical（2件）
interconnection-density / state-coupling

### linguistic（2件）
narrative-pressure / confession-mimicry

### economic（2件）
sunk-commitment / dominant-defection

### evolutionary（0件、未着手）
拡張候補: reciprocity-norm / status-anxiety / threat-detection-bias

---

## v0.3 既存composition辞書（参照用）

| Pattern | Composition |
|---|---|
| causal-misattribution | temporal-proximity-bias × visibility-asymmetry × narrative-pressure |
| escalation | intent-uncertainty × face-investment × sunk-commitment |
| authority-inversion | legitimacy-source-shift × capability-accumulation-asymmetry × incumbent-rigidity |
| cascade | interconnection-density × state-coupling × damping-absence |
| hubris-nemesis | success-blindness × feedback-suppression × scale-mismatch |
| groupthink | conformity-pressure × dissent-suppression × illusion-of-unanimity |
| decision-delegation-desire | responsibility-aversion × complexity-overwhelm × authority-availability |
| mission-drift | measurable-displacement × stakeholder-multiplication × founder-distance |
| chilling-effect | exemplary-visibility × identification-mirror × rule-ambiguity |
| judgment-evaporation | agentless-substitute × confession-mimicry × alibi-projection |
| prisoners-dilemma | dominant-defection × commitment-impossibility × non-iteration |
| founders-curse | charisma-institution-incompatibility × success-redefines-need × identity-lock |
| **algorithmic-abdication** | scale-mismatch × responsibility-aversion × complexity-overwhelm × authority-availability ★ atom由来初パターン |

---

## File Locations

```
dictionary/atoms/
├── _index.md           ← 索引・format spec・登録状況
├── atoms-graph.md      ← 関係マップ・新パターン候補
└── {atom-id}.md        ← 各atom（v0.3で36件）

dictionary/patterns/
└── {pattern-id}.md     ← composition block追記（v0.3で13件分解済）

memory/
├── MEMORY.md           ← レイヤー表更新
└── project_atoms_layer.md  ← 進捗ログ
```

---

## Working Examples（実行手順の参考）

### 例1: 新パターン分解（Mode 1）

ユーザー: `/atom-decompose mission-drift`

```
1. patterns/mission-drift.md を読む
2. 発動条件4つ（成長/ステークホルダー/短期圧/原点距離）を見る
3. 3つの独立atomを抽出:
   - measurable-displacement (institutional, Goodhart的駆逐)
   - stakeholder-multiplication (institutional, 関与者増殖)
   - founder-distance (institutional, 原点情報劣化)
4. 各atomファイル作成 (atoms/{name}.md)
5. patterns/mission-drift.md に composition block追加
6. _index.md と MEMORY 更新
```

### 例2: 新パターン演繹（Mode 2）

ユーザー: `/atom-decompose --derive`

```
1. atoms/_index.md から36 atoms確認
2. 既存13 patternの composition と重複しない組み合わせ生成
3. scale-mismatch × responsibility-aversion × complexity-overwhelm × authority-availability を発見
4. これは decision-delegation-desire の組織スケール拡張形
5. 既存事象（Robodebt, SyRI, COMPAS, A-level）にマッチ
6. 仮称 algorithmic-abdication で dictionary/patterns/algorithmic-abdication.md 登録
7. atoms-graph.md と _index.md を更新
```

### 例3: atom分解型記事（Mode 4）

ユーザー: `/atom-decompose --article algorithmic-abdication`

```
1. 該当patternの composition を確認
2. 4つのatom にすべてマッチする現代事象を選ぶ（Robodebt等）
3. 8セクション記事執筆:
   §1 ニュース概要 — Robodebt
   §2 一般的なフィルター — AIガバナンス論の薄さ
   §3 構造の抽出 — pattern + formula
   §4 問い — 「組織はいつ判断者をやめたのか？」
   §5 4つの原子 — 各atomを順に解剖
   §6 現状認識 — 2x2 + 業界横断テーブル
   §7 行動 — atom単位介入 + 組み合わせ介入
   §8 メタ — 4つの時間軸の収束として読み直し
4. articles/day-XXX-{pattern-id}.md に保存
5. フッターに反証条件と接続記述
```

---

## 100日KOSとの統合

このスキルは **100-day-kos** のサブツール。Day記事執筆で:

- **atom分解で深さを出したい時** → Mode 4
- **新パターンを発見した時** → Mode 1 で分解登録
- **複数Day記事の構造的接続が見えてきた時** → Mode 3 で graph更新

特に**atomic-abdication（Day 65）以降**、atom由来パターンを Day記事で扱う流れが定着すると、KOSの**自己拡張装置**として機能する。

---

## 反証条件（このスキル自体の）

以下が観察されたら、atom層の設計を再考する:

- ある事象が**5 atom以上**を必要とする → 4分割の限界。pattern再定義 or atom再分解
- 同じatomが**8 pattern以上**で使われ役割が散る → atom自体を分割すべき
- atomの介入点が空白で実装不能 → atom抽象が高すぎる
- 新パターン演繹が3ヶ月生まれない → 組み合わせ生成の自動化検討

---

## Memory（積み上げ用）

実行のたびに `memory/project_atoms_layer.md` に追記:

- 新規atom: name / domain / 関与pattern
- 新規分解: pattern / composition formula
- 新規演繹: 候補名 / atoms / マッチ事象
- 反省: domain偏重 / 重複検出 / 抽象すぎ など

---

## 出典

このスキルは2026-04-29のセッション「causal-misattribution が生まれた背景の前に何と何が掛け算されているか」という問いから発生。

- 初期動機: パターン解像度の低さ
- v0.1（9 atoms / 3 patterns）: prototype確立
- v0.2（21 atoms / 7 patterns）: domain拡張
- v0.3（36 atoms / 13 patterns）: 組織内動態カバー
- v0.4: スキル化（4 Modes 確立、`/atom-decompose` 利用可能化）
- v0.5: S+ テンプレ統合（Day 65 で C→S+ 検証完了、各セクションに動くスコア軸を明示）

詳細:
- `articles/day-065-algorithmic-abdication.md`（S+ 到達記事）
- `dictionary/atoms/atoms-graph.md`（21 atoms 関係マップ）
- `memory/feedback_atom_article_sranks.md`（critique打ち手リスト元）

---

#Skill #atom-decompose #knowledge-os #structure-resolution
