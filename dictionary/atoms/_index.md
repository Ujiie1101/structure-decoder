---
type: index
subtype: atoms
created: 2026-04-29
updated: 2026-05-13
status: prototype-v0.12
---

# Atoms — 構造の構成要素プリミティブ

## 目的

`patterns/` は中粒度の構造（210件）。本層はその**下位層**。
パターンを「**A × B × C の合成物**」として書き下したときの **A, B, C** にあたる原子を保管する。

```
事象（WWI、Theranos…）
  ↓ どんなpatternか
patterns/  ← 210件（中粒度）
  ↓ どんなatomの積か
atoms/     ← 本層（プリミティブ）
  ↓ そのatomは何由来か
（認知 / 物理 / 制度 / 言語 / 経済 / 進化）
```

## なぜ必要か

中粒度patternだけでは、以下の問いに答えられない:

1. **同じpatternが異なる時代・領域で再発する理由**は何か → 共通atomに帰着するから
2. **patternを壊すには何を消せばいいか** → atom単位の介入点を特定する
3. **新パターンの発見** → 既存atomの未試行の組み合わせ

## 命名規則

- `id`: kebab-case、英語、抽象名詞中心
- `name`: 日本語、12文字以内推奨
- `domain`: 起源の領域 — `cognitive` / `social` / `institutional` / `linguistic` / `physical` / `economic` / `evolutionary` のいずれか1つ

## ファイル構造

各atomファイル（`{id}.md`）の必須セクション:

```yaml
---
id: "..."
name: "..."
type: "atom"
domain: "cognitive"
created: 2026-04-29
---

# {name}

1段落の定義。

## 起源（Why this exists）
このatomが世界に存在する理由。進化・物理・制度・言語のどれに根ざすか。

## 観察可能なproxy
発動を検知する具体的シグナル。

## 介入点（Disable conditions）
このatomを打ち消す、または無効化する条件。

## 関与パターン
このatomが構成要素として登場するpattern一覧。
```

## composition記法（patterns側）

各 `patterns/{id}.md` の frontmatter に以下を追加可能:

```yaml
composition:
  - atom: temporal-proximity-bias
    role: 引き金の知覚を曇らせる
  - atom: visibility-asymmetry
    role: 構造を不可視化する
  - atom: narrative-pressure
    role: 物語化可能な原因を選択させる
```

`role` はそのatomがpattern内で果たす機能。同じatomが別patternでは別roleを持ちうる。

## 登録状況

### v0.1（2026-04-29）— 認知/社会/制度の三領域

| Domain | Atom | 関与pattern |
|---|---|---|
| cognitive | [temporal-proximity-bias](temporal-proximity-bias.md) | causal-misattribution |
| cognitive | [visibility-asymmetry](visibility-asymmetry.md) | causal-misattribution |
| linguistic | [narrative-pressure](narrative-pressure.md) | causal-misattribution |
| social | [intent-uncertainty](intent-uncertainty.md) | escalation |
| social | [face-investment](face-investment.md) | escalation |
| economic | [sunk-commitment](sunk-commitment.md) | escalation |
| institutional | [legitimacy-source-shift](legitimacy-source-shift.md) | authority-inversion |
| social | [capability-accumulation-asymmetry](capability-accumulation-asymmetry.md) | authority-inversion |
| institutional | [incumbent-rigidity](incumbent-rigidity.md) | authority-inversion |

### v0.2（2026-04-29）— ネットワーク/組織内動態

| Domain | Atom | 関与pattern |
|---|---|---|
| physical | [interconnection-density](interconnection-density.md) | cascade |
| physical | [state-coupling](state-coupling.md) | cascade |
| institutional | [damping-absence](damping-absence.md) | cascade |
| cognitive | [success-blindness](success-blindness.md) | hubris-nemesis |
| institutional | [feedback-suppression](feedback-suppression.md) | hubris-nemesis |
| cognitive | [scale-mismatch](scale-mismatch.md) | hubris-nemesis |
| social | [conformity-pressure](conformity-pressure.md) | groupthink |
| social | [dissent-suppression](dissent-suppression.md) | groupthink |
| cognitive | [illusion-of-unanimity](illusion-of-unanimity.md) | groupthink |
| cognitive | [responsibility-aversion](responsibility-aversion.md) | decision-delegation-desire |
| cognitive | [complexity-overwhelm](complexity-overwhelm.md) | decision-delegation-desire |
| institutional | [authority-availability](authority-availability.md) | decision-delegation-desire |

### v0.3（2026-04-29）— 漂流/萎縮/蒸発/ジレンマ/呪い

| Domain | Atom | 関与pattern |
|---|---|---|
| institutional | [measurable-displacement](measurable-displacement.md) | mission-drift |
| institutional | [stakeholder-multiplication](stakeholder-multiplication.md) | mission-drift |
| institutional | [founder-distance](founder-distance.md) | mission-drift |
| social | [exemplary-visibility](exemplary-visibility.md) | chilling-effect |
| cognitive | [identification-mirror](identification-mirror.md) | chilling-effect |
| institutional | [rule-ambiguity](rule-ambiguity.md) | chilling-effect |
| institutional | [agentless-substitute](agentless-substitute.md) | judgment-evaporation |
| linguistic | [confession-mimicry](confession-mimicry.md) | judgment-evaporation |
| cognitive | [alibi-projection](alibi-projection.md) | judgment-evaporation |
| economic | [dominant-defection](dominant-defection.md) | prisoners-dilemma |
| institutional | [commitment-impossibility](commitment-impossibility.md) | prisoners-dilemma |
| social | [non-iteration](non-iteration.md) | prisoners-dilemma |
| institutional | [charisma-institution-incompatibility](charisma-institution-incompatibility.md) | founders-curse |
| social | [success-redefines-need](success-redefines-need.md) | founders-curse |
| cognitive | [identity-lock](identity-lock.md) | founders-curse |

### v0.7（2026-04-29）— evolutionary 領域開拓

| Domain | Atom | 関与pattern |
|---|---|---|
| evolutionary | [reciprocity-norm](reciprocity-norm.md) | prisoners-dilemma / coordination-failure（進化的下地） |
| evolutionary | [status-anxiety](status-anxiety.md) | face-investment / conformity-pressure / hubris の進化的根 |
| evolutionary | [threat-detection-bias](threat-detection-bias.md) | identification-mirror の進化的下地 |
| evolutionary | [dunbar-limit](dunbar-limit.md) | scale-mismatch の生物学的根拠 |
| evolutionary | [in-group-bias](in-group-bias.md) | conformity-pressure / exemplary-visibility の進化的根拠 |

これらは既存atomの**進化的下地**として機能する。新規パターン分解には未投入だが、既存atomの理解を深める形で組み込まれる。

### v0.8（2026-04-30）— 集団記憶層 / 疫学的忘却

| Domain | Atom | 関与pattern |
|---|---|---|
| social | [generational-amnesia](generational-amnesia.md) | epidemiological-amnesia（Day66、atom由来第2パターン） |

### v0.9（2026-05-06）— 軸atom（道具選定の隠れ軸）

| Domain | Atom | 関与pattern |
|---|---|---|
| physical | [programmability-as-axis](programmability-as-axis.md) | surface-axis-occlusion（道具選定の量産性軸） |
| institutional | [ownership-vs-access](ownership-vs-access.md) | surface-axis-occlusion（道具選定の独立性軸） |

両 atom は「メカニズム原子」ではなく「軸（dimension）原子」という変則種。surface-axis-occlusion パターンが指示する**隠される軸**の典型例として登録。daily-writing skill 経由で発見された最初の atom 群。

### v0.10（2026-05-12）— 制度的剥離 / コンテキスト断絶

| Domain | Atom | 関与pattern |
|---|---|---|
| institutional | [context-stripping](context-stripping.md) | capture（脱文脈化副概念のatom化）/ institutionalization / focal-point-absence / articulation-residue |

daily-writing skill 経由で発見。`200_Output/substack-daily/2026-05-12-clock-and-parental-education.md`（小学2年生の娘が時計の午前/午後を理解できない違和感）から派生。学校教育・ニュース・テスト・行政掲示・カタログなど制度全般に横断する基底動作「情報を点に剥離する」を atom 化。既存 capture パターンの副概念「脱文脈化」を atom レベルへ独立させた。

### v0.11（2026-05-13）— 言語による告発不能攻撃の生態系（坊っちゃん全11章由来）

| Domain | Atom | 関与pattern |
|---|---|---|
| linguistic | [calibrated-audibility](calibrated-audibility.md) | un-accusable-attack / innuendo-broadcast |
| linguistic | [borrowed-pedigree](borrowed-pedigree.md) | un-accusable-attack / innuendo-broadcast / logic-barrage |
| social | [arsonist-firefighter-identity](arsonist-firefighter-identity.md) | un-accusable-attack / apology-rhetoric-solo-circulation |
| linguistic | [adjective-arrow](adjective-arrow.md) | un-accusable-attack / triangulation-attack / innuendo-broadcast |
| social | [silent-norm-update](silent-norm-update.md) | un-accusable-attack / apology-rhetoric-solo-circulation |
| social | [frontal-method-purity](frontal-method-purity.md) | un-accusable-attack 対抗装置 / mediator-trap-fallback |
| social | [second-information-axis](second-information-axis.md) | un-accusable-attack 対抗装置 / auto-completion-of-suggestion 阻害 |
| social | [kindness-intrusion](kindness-intrusion.md) | bait-substitution |

book-series skill による 夏目漱石『坊っちゃん』全11章 (1906) の構造分解から派生。組織における「告発できない攻撃」の生態系を構成する基底動作 8件を atom 化。各 atom は MeToo・SLAPP訴訟・社内政治・SNS炎上など 2026年現代事象の解析にも適用可能。

### v0.12（2026-05-13）— 没落・書字・継承の生態系（斜陽全八章由来）

| Domain | Atom | 関与pattern |
|---|---|---|
| linguistic | [sign-long-distance-recovery](sign-long-distance-recovery.md) | disappearance-emergence-synchrony / delayed-delivery-as-education |
| linguistic | [writing-irreversibility](writing-irreversibility.md) | simultaneous-contradiction-operation / tragedy-to-comedy-dispatch |
| linguistic | [addressee-postvariation](addressee-postvariation.md) | simultaneous-contradiction-operation |
| cognitive | [spiral-of-past](spiral-of-past.md) | delayed-delivery-as-education |
| social | [inheritance-unidirectionality](inheritance-unidirectionality.md) | disappearance-emergence-synchrony / tragedy-to-comedy-dispatch |
| social | [family-vitality-conservation](family-vitality-conservation.md) | disappearance-emergence-synchrony |
| social | [deviant-tenderness](deviant-tenderness.md) | pseudo-thought-from-bar |
| cognitive | [retroactive-origin-acceptance](retroactive-origin-acceptance.md) | tragedy-to-comedy-dispatch |

book-series skill による 太宰治『斜陽』全八章 (1947) の構造分解から派生。「没落／書字／継承／反転」の生態系を構成する基底動作 8件を atom 化。書物全体を貫通する徴候の長距離回収（蛇→母の死→書名反転）、第四章＝第七章の書字対称、第八章の喜劇化送信など、戦後文学の核心的装置を抽出。各 atom は事業承継・移民2世アイデンティティ・SNS書字文化など 2026年現代事象の解析にも適用可能。

なお同じ斜陽から派生した **book-level の操作技法** 2件（chapter-pivot-line / title-self-inversion）は、event-level atom と区別して [135_Meta/book-level-techniques/](../../135_Meta/book-level-techniques/_index.md) に格納。書き手側の編集技法として別レイヤー扱い。

**累計**: 77 atoms / 33 patterns 分解済 / 2 meta-atoms（135_Meta/ 配下）

### 分解済パターン総覧

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
| unintended-consequences | causal-distance × second-order-blindness × agent-multiplicity |
| bystander-economics | action-cost-asymmetry × prevention-invisibility × responsibility-diffusion |
| coordination-failure | strategic-complementarity × common-knowledge-gap × focal-point-absence |
| output-less-critique | alternative-cost × empathy-incentive × stake-free-visibility |
| **mechanization-resistance** | gap-awareness × assimilation-rejection × articulation-residue ★ atom由来第2パターン（観察主体の自己同定から演繹） |
| **epidemiological-amnesia** | success-blindness × generational-amnesia × legitimacy-source-shift × narrative-pressure ★ atom由来第3パターン（公衆衛生成功の自己侵食、Day66） |
| **surface-axis-occlusion** | programmability-as-axis ⊕ ownership-vs-access ★ daily-writing由来初パターン（流通する比較フレームが文脈依存軸を覆う、2026-05-06）。変則構成：composition は「隠される軸」を atom として記録。メカニズム原子（comparability-asymmetry / distribution-incentive / context-blindness）の登録は次フェーズ |
| **un-accusable-attack** | calibrated-audibility × adjective-arrow × arsonist-firefighter-identity × silent-norm-update ★ book-series由来メタパターン（坊っちゃん全11章貫通、2026-05-13） |
| **innuendo-broadcast** | calibrated-audibility × adjective-arrow ★ book-series由来（第三者前での匂わせ三要素、第五章） |
| **triangulation-attack** | adjective-arrow × responsibility-aversion ★ book-series由来（媒介を通した攻撃、第五・六章） |
| **auto-completion-of-suggestion** | adjective-arrow × narrative-pressure ★ book-series由来（時間経過による暗示の自己完成、第六章） |
| **bait-substitution** | kindness-intrusion × arsonist-firefighter-identity ★ book-series由来（A排除→B懐柔、第八章） |
| **mediator-trap-fallback** | frontal-method-purity × responsibility-aversion ★ book-series由来（仲裁者が制度的に罰せられる、第十章） |
| **accusation-asymmetry** | stake-free-visibility × face-investment ★ book-series由来（MeToo構造、第十一章） |
| **apology-rhetoric-solo-circulation** | arsonist-firefighter-identity × silent-norm-update ★ book-series由来（謝罪と処分の分離、第六・十章） |
| **disappearance-emergence-synchrony** | inheritance-unidirectionality × sign-long-distance-recovery × family-vitality-conservation ★ book-series由来（斜陽第五章・母の死と革命家宣言の同時性、2026-05-13） |
| **delayed-delivery-as-education** | spiral-of-past × generational-amnesia × sign-long-distance-recovery ★ book-series由来（斜陽第三章・教育の遅延配達） |
| **simultaneous-contradiction-operation** | writing-irreversibility × addressee-postvariation × confession-mimicry ★ book-series由来（斜陽第四章・三通の手紙の矛盾運用） |
| **tragedy-to-comedy-dispatch** | retroactive-origin-acceptance × writing-irreversibility × inversion ★ book-series由来（斜陽第八章・「マイ・コメデアン」） |
| **pseudo-thought-from-bar** | borrowed-pedigree × confession-mimicry × deviant-tenderness ★ book-series由来（斜陽第七章・直治の遺書） |

## 次の拡張候補

### atom候補（未登録）
- `attention-finiteness`（注意の有限性）
- `coordination-cost`（協調コスト）
- `time-discount`（時間割引）
- `reciprocity-norm`（互恵規範）
- `commitment-irreversibility`（コミットメント不可逆性）

これらは複数patternに横断的に登場する見込み。

### 分解候補pattern（次の優先候補）
- `unintended-consequences`（意図せざる結果）
- `coordination-failure`（協調失敗）
- `bystander-economics`（傍観者経済学）
- `output-less-critique`（無出力批判）
- `regulatory-capture`（規制捕獲）
- `network-parasitism`（ネットワーク寄生）
- `pain-downstream-deposit`（痛みの下流預託）
- `child-shield`（子盾）
- `parental-deposit`（親預託）
- `self-tipping`（自己転倒）

## atom間の関係グラフ

詳細は **[atoms-graph.md](atoms-graph.md)** 参照。

含まれる内容:
- ドメイン分布
- 共起グラフ（Mermaid）
- 隣接ペア（似て非なる8組）
- 相補論理（pattern内三項の論理積）
- 循環ループ3件（groupthink自己強化 / 委託需給拡張 / escalation累積）
- 介入atom候補22件（atom破壊用）
- 横断利用候補
- **新パターン候補10件**（未試行のatom組み合わせから生成）

最優先候補: `algorithmic-abdication`（scale-mismatch × responsibility-aversion × authority-availability × complexity-overwhelm）— AI時代の構造
