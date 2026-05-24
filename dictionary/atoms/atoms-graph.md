---
type: graph
subtype: atoms-relationships
created: 2026-04-29
updated: 2026-05-11
status: prototype-v0.9
atom_count: 60
pattern_count: 20
atom_derived_patterns: 4
domains_covered: 7/7（全領域到達）
---

# Atoms Graph v0.7 — atom間の関係性マップ

## 目的

56 atoms（v0.1〜v0.7、全7 domain）の関係を整理し、

1. **既存パターン**を atom組み合わせで再構成
2. **未試行の組み合わせ**から新パターン候補を抽出
3. **介入関係**（atom A を消す atom B）を可視化
4. **対称性ペア**（似て非なる atom）を文書化（v0.6 発見）
5. **進化的下地ペア**（社会/認知 atom の進化的根拠）を文書化（v0.7 発見）

---

## ドメイン分布（v0.7、全7領域到達）

| Domain | Count | % | Atoms |
|---|---|---|---|
| cognitive | 14 | 27% | temporal-proximity-bias / visibility-asymmetry / success-blindness / scale-mismatch / illusion-of-unanimity / responsibility-aversion / complexity-overwhelm / identification-mirror / alibi-projection / identity-lock / second-order-blindness / prevention-invisibility / gap-awareness / assimilation-rejection |
| social | 13 | 25% | intent-uncertainty / face-investment / capability-accumulation-asymmetry / conformity-pressure / dissent-suppression / exemplary-visibility / non-iteration / success-redefines-need / agent-multiplicity / responsibility-diffusion / common-knowledge-gap / empathy-incentive / stake-free-visibility |
| institutional | 13 | 25% | legitimacy-source-shift / incumbent-rigidity / damping-absence / feedback-suppression / authority-availability / measurable-displacement / stakeholder-multiplication / founder-distance / rule-ambiguity / agentless-substitute / commitment-impossibility / charisma-institution-incompatibility / focal-point-absence |
| economic | 5 | 10% | sunk-commitment / dominant-defection / action-cost-asymmetry / strategic-complementarity / alternative-cost |
| physical | 3 | 6% | interconnection-density / state-coupling / causal-distance |
| linguistic | 3 | 6% | narrative-pressure / confession-mimicry / articulation-residue |
| evolutionary | 5 | 9% | reciprocity-norm / status-anxiety / threat-detection-bias / dunbar-limit / in-group-bias |

**v0.2→v0.7 の進化**: cognitive 33%→25%（偏重緩和）、economic 5%→9%（約2倍）、**evolutionary 0%→9%（v0.7 で開拓完了）**。全7 domain 到達済。次の優先は physical / linguistic の拡張。

---

## 18 patterns × composition 完全リスト

| # | Pattern | Composition | 備考 |
|---|---|---|---|
| 1 | causal-misattribution | temporal-proximity-bias × visibility-asymmetry × narrative-pressure | v0.1 |
| 2 | escalation | intent-uncertainty × face-investment × sunk-commitment | v0.1 |
| 3 | authority-inversion | legitimacy-source-shift × capability-accumulation-asymmetry × incumbent-rigidity | v0.1 |
| 4 | cascade | interconnection-density × state-coupling × damping-absence | v0.2 |
| 5 | hubris-nemesis | success-blindness × feedback-suppression × scale-mismatch | v0.2 |
| 6 | groupthink | conformity-pressure × dissent-suppression × illusion-of-unanimity | v0.2 |
| 7 | decision-delegation-desire | responsibility-aversion × complexity-overwhelm × authority-availability | v0.2 |
| 8 | mission-drift | measurable-displacement × stakeholder-multiplication × founder-distance | v0.3 |
| 9 | chilling-effect | exemplary-visibility × identification-mirror × rule-ambiguity | v0.3 |
| 10 | judgment-evaporation | agentless-substitute × confession-mimicry × alibi-projection | v0.3 |
| 11 | prisoners-dilemma | dominant-defection × commitment-impossibility × non-iteration | v0.3 |
| 12 | founders-curse | charisma-institution-incompatibility × success-redefines-need × identity-lock | v0.3 |
| 13 | **algorithmic-abdication** | scale-mismatch × responsibility-aversion × complexity-overwhelm × authority-availability | ★ atom由来① (Day65) |
| 14 | unintended-consequences | causal-distance × second-order-blindness × agent-multiplicity | v0.6 |
| 15 | bystander-economics | action-cost-asymmetry × prevention-invisibility × responsibility-diffusion | v0.6 |
| 16 | coordination-failure | strategic-complementarity × common-knowledge-gap × focal-point-absence | v0.6 |
| 17 | output-less-critique | alternative-cost × empathy-incentive × stake-free-visibility | v0.6 |
| 18 | **mechanization-resistance** | gap-awareness × assimilation-rejection × articulation-residue | ★ atom由来② / 観察主体由来 |
| 19 | **epidemiological-amnesia** | success-blindness × generational-amnesia × legitimacy-source-shift × narrative-pressure | ★ atom由来③ (Day66) |
| 20 | **prevention-self-erasure** | prevention-invisibility × experiential-amnesia (× generational-amnesia bg) | ★ atom由来④ / daily-writing由来② (Day72) |

---

## 進化的下地ペア（v0.7 新規発見）

evolutionary atom は単独で機能するというより、**既存 social/cognitive atom の進化的根拠**として機能する。これにより既存atomの「なぜそうなるか」が深く説明できる。

| 既存 atom（表層） | 進化的下地（深層） | 説明 |
|---|---|---|
| **face-investment** | status-anxiety | 公的撤退コストの根は地位喪失への進化的恐怖 |
| **conformity-pressure** | status-anxiety + in-group-bias | 同調は地位維持と内集団残留の二重戦略 |
| **dissent-suppression** | in-group-bias | 異論者を「外」に押し出す進化的反応 |
| **identification-mirror** | threat-detection-bias | 他者の被害を自己投影するのは捕食者検知の延長 |
| **exemplary-visibility** | threat-detection-bias + in-group-bias | 内集団内の見せしめは強烈、外集団のは効果薄 |
| **scale-mismatch** | dunbar-limit | 規模超過の生物学的根拠は150人の認知容量 |
| **complexity-overwhelm** | dunbar-limit | 関係性の処理限界が複雑性の主源 |
| **non-iteration** | reciprocity-norm（の不在） | 反復ゲームでは互恵が機能、一回限りで崩壊 |
| **hubris** | status-anxiety の過剰補正 | 地位上昇後の不安解除が暴走する形 |
| **dominant-defection** | reciprocity-norm の停止 | 互恵が切れた状況での合理戦略 |

### 含意

evolutionary atom は **抽象 atom の根**として全層に浸透する:

```
進化的下地（v0.7）
   ↓
社会/認知 atom（v0.1-0.6）
   ↓
patterns（17 + 第四項）
   ↓
事象（Robodebt、SyRI、観察主体の自己同定…）
```

この四層構造は、KOS の説明力を**進化的時間軸（数十万年）**にまで拡張する。

---

## 対称性ペア（v0.6 発見）

似て非なる atom は混同回避のため独立に登録されてきたが、**対称性を持つペア**として整理すると、構造の理解が深まる。

### 主要対称ペア

| ペアA | ペアB | 対称性の軸 |
|---|---|---|
| **success-blindness** | **gap-awareness** | 自己バイアスの濃淡（過信 vs 直視） |
| **conformity-pressure** | **assimilation-rejection** | 集団動態への向き（同調 vs 拒否） |
| **confession-mimicry** | **articulation-residue** | 言語の射程（語りすぎ vs 語れない） |
| **responsibility-aversion** | **responsibility-diffusion** | 責任問題の所在（個人内 vs 集団内） |
| **visibility-asymmetry** | **prevention-invisibility** | 不可視性の対象（構造 vs 反実仮想） |
| **intent-uncertainty** | **common-knowledge-gap** | 情報の階層（直接情報 vs メタ情報） |
| **exemplary-visibility** | **stake-free-visibility** | 可視性の方向（罰される側 vs 罰されない側） |
| **alibi-projection** | **articulation-residue** | 不在への対処（投影 vs 直視） |

### 対称性の含意

これらの対称ペアは、**対立する人間条件**を表す:

- **過信 → 化石化** vs **直視 → 抵抗**
- **同調 → 凡庸** vs **拒否 → 残余**
- **語りすぎ → AI** vs **語れなさ → 人間**

つまり、Day 64 / Day 65 の批判側 atom と、Day 65 終盤〜mechanization-resistance の抵抗側 atom が、**鏡像として対をなしている**。これは KOS が、現象の批判だけでなく、**抵抗者の自己同定**まで構造化できる証拠。

---

## 循環ループ（既知 + v0.6 新規）

### 既知3ループ

1. **groupthink 自己強化**: dissent-suppression → conformity-pressure → 沈黙 → illusion-of-unanimity → 過去の罰の正当化
2. **委託需給拡張**: responsibility-aversion + complexity-overwhelm → authority-availability ↑ → 委託閾値 ↓
3. **escalation 累積**: intent-uncertainty → face-investment → sunk-commitment → さらなる face-investment

### v0.6 新規ループ

4. **bystander-economics 自己強化**:
   ```
   action-cost-asymmetry（高コスト）
       ↓
   傍観選択
       ↓
   prevention-invisibility（防いだ被害が見えない）
       ↓
   行動の便益が認識されない
       ↓
   さらなる action-cost-asymmetry の固定化（行動者がいない）
   ```

5. **output-less-critique 自己拡大**:
   ```
   alternative-cost（高コスト）→ 批判のみ発信
       ↓
   empathy-incentive で報酬獲得
       ↓
   stake-free-visibility で目立つ
       ↓
   さらなる批判発信が報酬される
       ↓
   代案発信者は埋没
   ```

6. **mechanization-resistance 強化（自己肯定的）**:
   ```
   gap-awareness（直視）
       ↓
   assimilation-rejection（拒否）
       ↓
   articulation-residue（語れなさの自覚）
       ↓
   gap-awareness のさらなる深化
   ```
   ※他の循環と異なり、**抵抗者の position を強化する正の循環**。第四項に立ち続ける機構。

---

## 介入 atom（counter-atom）一覧（v0.6 拡張）

各 atom を打ち消す介入候補。51 atoms すべてに counter が定義可能だが、特に重要な対応:

| Atom | 介入 atom（counter候補） |
|---|---|
| temporal-proximity-bias | base-rate-anchoring |
| visibility-asymmetry | structure-rendering |
| narrative-pressure | meta-narrative |
| intent-uncertainty | transparency-protocol |
| face-investment | face-saving-exit |
| sunk-commitment | sunset-clause |
| legitimacy-source-shift | source-incorporation |
| capability-accumulation-asymmetry | mutual-learning |
| incumbent-rigidity | external-injection |
| interconnection-density | compartmentalization |
| state-coupling | buffer-insertion |
| damping-absence | circuit-breaker |
| success-blindness | failure-archive |
| feedback-suppression | bypass-channel |
| scale-mismatch | downsize-or-augment |
| conformity-pressure | anonymization |
| dissent-suppression | dissent-rewarding |
| illusion-of-unanimity | private-polling |
| responsibility-aversion | process-evaluation |
| complexity-overwhelm | choice-curation |
| authority-availability | authority-pluralization |
| measurable-displacement | qualitative-mandate |
| stakeholder-multiplication | mission-hierarchy |
| founder-distance | origin-ritualization |
| exemplary-visibility | private-resolution |
| identification-mirror | dissimilation-narrative |
| rule-ambiguity | rule-clarification |
| agentless-substitute | tool-framing |
| confession-mimicry | mimicry-annotation |
| alibi-projection | signature-discipline |
| dominant-defection | payoff-restructuring |
| commitment-impossibility | binding-mechanism |
| non-iteration | reputation-system |
| charisma-institution-incompatibility | dual-track |
| success-redefines-need | role-redefinition |
| identity-lock | identity-multiplication |
| **causal-distance**（v0.6） | causal-mapping |
| **second-order-blindness**（v0.6） | system-thinking-training |
| **agent-multiplicity**（v0.6） | agent-based-simulation |
| **action-cost-asymmetry**（v0.6） | action-subsidy / inaction-penalty |
| **prevention-invisibility**（v0.6） | counterfactual-quantification |
| **responsibility-diffusion**（v0.6） | individual-naming |
| **strategic-complementarity**（v0.6） | independence-incentive |
| **common-knowledge-gap**（v0.6） | public-announcement |
| **focal-point-absence**（v0.6） | focal-point-declaration |
| **alternative-cost**（v0.6） | alternative-mandate |
| **empathy-incentive**（v0.6） | insight-incentive |
| **stake-free-visibility**（v0.6） | skin-in-the-game |
| **gap-awareness**（v0.6） | ※打ち消すべきではない |
| **assimilation-rejection**（v0.6） | ※打ち消すべきではない |
| **articulation-residue**（v0.6） | ※打ち消すべきではない |
| **reciprocity-norm**（v0.7） | ※基本的に保護すべき／悪用ループは止める |
| **status-anxiety**（v0.7） | meaning-pluralization / 比較対象選択の自覚 |
| **threat-detection-bias**（v0.7） | base-rate-grounding / メディアダイエット |
| **dunbar-limit**（v0.7） | ※認知容量なので超えられない／規模縮小しかない |
| **in-group-bias**（v0.7） | superordinate-goal / contact-hypothesis |

**重要**: mechanization-resistance を構成する3 atom は、**打ち消すべきではない**。これは「壊すと第四項の人間が消える」という意味で、システム的に保護対象。

---

## 横断利用 atom（複数 pattern にまたがる）

以下の atom は、登録時の pattern以外でも作動が確認できる。今後 cross-pattern 注釈の対象:

| Atom | 主登録 pattern | 横断登場 pattern |
|---|---|---|
| scale-mismatch | hubris-nemesis | algorithmic-abdication ✓ / mission-drift / judgment-evaporation |
| feedback-suppression | hubris-nemesis | mission-drift / groupthink |
| visibility-asymmetry | causal-misattribution | bystander-economics（隣接） / chilling-effect |
| face-investment | escalation | chilling-effect / output-less-critique |
| damping-absence | cascade | bystander-economics（介入機構欠如） |
| narrative-pressure | causal-misattribution | mission-drift / output-less-critique |
| sunk-commitment | escalation | mission-drift / hubris-nemesis |
| authority-availability | DDD | algorithmic-abdication ✓ / vacuum-authoritarian-cycle |
| responsibility-aversion | DDD | algorithmic-abdication ✓ / output-less-critique（隣接） |
| complexity-overwhelm | DDD | algorithmic-abdication ✓ / mission-drift（隣接） |

---

## 未試行の組み合わせ → 新パターン候補（v0.6 拡張）

51 atoms から、既存18 patternに含まれない有望な組み合わせ7件:

### 候補1: `historical-responsibility-evaporation`（歴史責任蒸発）

**Composition**: causal-distance × responsibility-diffusion × narrative-pressure

数十年の時を経た歴史責任が、責任拡散と物語化で蒸発する構造。

**典型例**: 戦争責任、植民地責任、世代間負債、企業の長期スキャンダル
**親pattern**: judgment-evaporation の歴史軸特殊形
**優先度**: 高

---

### 候補2: `critic-trap`（批評家の罠）

**Composition**: gap-awareness × stake-free-visibility × empathy-incentive

ギャップを直視できるがゆえに批評する力を持つ人が、賭けなき可視性と共感報酬の構造に絡め取られる罠。

**典型例**: 学者の言論市場化、評論家のSNS化、批判で食う知識人の構造的堕落
**親pattern**: output-less-critique の能力者特殊形
**優先度**: 中〜高（user の警戒すべき位置として）

---

### 候補3: `aware-abdication`（自覚ある放棄）

**Composition**: gap-awareness × authority-availability × responsibility-aversion

ギャップを自覚しながらも、それゆえにこそ AI に頼らざるを得ない人の構造。**第四項に至れない多数派**の位置。

**典型例**: AI を使うと罪悪感を持ちながら使い続ける専門職、判断委譲を「合理的選択」と説明する自分
**親pattern**: algorithmic-abdication の自覚有特殊形
**優先度**: 最高（社会の99%が該当する可能性）

---

### 候補4: `safety-sinkhole`（安全部門沈降）

**Composition**: prevention-invisibility × measurable-displacement × responsibility-diffusion

安全・予防・コンプライアンス部門が、測定不能な成果と分散責任で組織内で沈降する構造。

**典型例**: 安全部門の予算削減、コンプラ部門の形骸化、品質管理の縮小
**親pattern**: bystander-economics × mission-drift のハイブリッド
**優先度**: 中

---

### 候補5: `incumbent-convergence`（既得権益収斂）

**Composition**: strategic-complementarity × common-knowledge-gap × authority-availability

複数均衡が存在するが、既得権益が**事実上の focal point**として機能し、改革困難な均衡に固定される構造。

**典型例**: 政治改革の停滞、業界慣習、組織内の暗黙ルール
**親pattern**: coordination-failure の権力不均衡特殊形
**優先度**: 中

---

### 候補6: `observer-economy`（観察者経済）

**Composition**: action-cost-asymmetry × empathy-incentive × stake-free-visibility

「批判するが行動しない、共感を集めるが賭けない」現代的観察者像の経済構造。

**典型例**: SNSインフルエンサー、評論家、社会派ライター（の最悪形態）
**親pattern**: output-less-critique × bystander-economics のハイブリッド
**優先度**: 高（時代記述として）

---

### 候補7: `articulation-paradox`（言語化の逆説、v0.6）

**Composition**: confession-mimicry × articulation-residue × empathy-incentive

AI が代わりに語ってくれる時代、人間の語れなさが**かえって価値を持つ**構造の逆説。AI ほど語れない人の言葉が、AI が再現できない深さを持つ。

**典型例**: 現代の優れた哲学エッセイ、言語化苦闘の自伝
**親pattern**: mechanization-resistance の生産的特殊形
**優先度**: 中（user の100日KOSプロジェクトそのものの構造）

---

### 候補8: `tribal-cooperation-limit`（部族協力の限界、v0.7）

**Composition**: reciprocity-norm × dunbar-limit × in-group-bias

人類の協力は150人以下の内集団では機能するが、それを超えると**機械化（制度・官僚制・AI）**に頼るしかなくなる構造。

**典型例**: 都市国家から帝国への遷移、ベンチャーから大企業への変質、グローバル化の機械的調整依存
**親pattern**: algorithmic-abdication の生物学的説明形 / scale-mismatch の進化的理由
**優先度**: 高（人類史の射程を持つ）

---

### 候補9: `scapegoat-formation`（スケープゴート形成、v0.7）

**Composition**: threat-detection-bias × in-group-bias × narrative-pressure

外集団に脅威を投影し、物語化して**集団の罪を一身に負わせる**構造。多くの歴史的虐殺・差別の核。

**典型例**: 魔女狩り、ナチス・ドイツのユダヤ人迫害、ルワンダ虐殺、SNS の「炎上対象」
**親pattern**: chilling-effect の極端形 / causal-misattribution × in-group-bias の合成
**優先度**: 高（歴史記述・予防論として）

---

### 候補10: `status-driven-abdication`（地位駆動型放棄、v0.7）

**Composition**: status-anxiety × authority-availability × responsibility-aversion

地位を失いたくないから AI に判断させる。「専門家として外れた判断をした」と評されるリスクを避けるため、AI 判定を**地位防衛装置**として使う構造。

**典型例**: AI 判定に従う医師（医療訴訟回避）／AI 推奨に従うコンサル（クライアント説明容易化）／AI スコアに従う投資家
**親pattern**: algorithmic-abdication の動機特殊形（status-anxiety を加えた4-atom）
**優先度**: 最高（algorithmic-abdication の進化的補強として）

---

## 候補評価マトリクス

| 候補 | 既存pattern との関係 | 記事化適性 | 登録優先度 |
|---|---|---|---|
| historical-responsibility-evaporation | judgment-evaporation 派生 | 高（戦後責任論） | 高 |
| **critic-trap** | output-less-critique 派生 | 高（自己警戒） | 高 |
| **aware-abdication** | algorithmic-abdication 派生 | **最高** | **最高** |
| safety-sinkhole | bystander × mission-drift | 中 | 中 |
| incumbent-convergence | coordination-failure 派生 | 中 | 中 |
| **observer-economy** | output-less × bystander | **最高** | **高** |
| articulation-paradox | mechanization-resistance 派生 | 高（自己再帰） | 中 |
| **tribal-cooperation-limit** | algorithmic-abdication の進化的説明 | 最高（人類史） | 高 |
| **scapegoat-formation** | chilling-effect 極端形 | 最高（歴史・予防） | 高 |
| **status-driven-abdication** | algorithmic-abdication 動機特殊形 | **最高** | **最高** |

---

## v0.6→v0.7 で見えてきた構造

### 1. 対称性が KOS の二極化を可視化（v0.6）

56 atoms は、**批判・分析側**と**抵抗・残余側**の二極を持つ。Day 64-65 で批判側を強化し、Day 65 終盤〜mechanization-resistance で抵抗側を構造化した。

### 2. 観察主体の自己同定が pattern として登録可能に（v0.6）

mechanization-resistance は **user の自己同定**から演繹された。これは KOS が「他者・社会の観察」だけでなく「**観察者自身の position**」も構造化できる装置に進化したことを意味する。

### 3. 経済 atom が 5 倍に成長（v0.6）

v0.2 では 1 atom（sunk-commitment）だけだった経済領域が、5 atomsに。bystander-economics / coordination-failure / output-less-critique の追加で経済構造の解像度が上がった。

### 4. 進化的下地で四層構造が完成（v0.7）

evolutionary 領域 5件追加で全7 domain網羅。これにより、KOS は**四層**で説明可能になった:

```
進化的下地（数十万年スケール）
    ↓
社会/認知 atom（数百年〜数十年）
    ↓
patterns（中粒度構造）
    ↓
事象（具体例）
```

特に重要な接続:
- **face-investment ← status-anxiety**：地位への進化的恐怖が公的撤退コストの根
- **scale-mismatch ← dunbar-limit**：規模超過の生物学的限界
- **identification-mirror ← threat-detection-bias**：捕食者検知の現代的誤発火

### 5. 進化的視座で algorithmic-abdication が再解釈される（v0.7）

`tribal-cooperation-limit`（候補8）が示唆する深い構造:

> **人類の協力は150人で頭打ち。それ以上の規模を扱うには、機械化に頼るしかない**

algorithmic-abdication（Day 65）は「組織が判断者をやめた」と批判されたが、進化的視座では**dunbar-limit を超えた集団における必然的選択**でもある。これはユーザーが提起した「権限譲渡は最適解になりうる」哲学的問いに、**進化生物学が裏付けを与える**形になる。

ただし、これは abdication を肯定するのではなく、**「abdication せざるを得ない人類条件」の構造的説明**として機能する。批判から記述へ、記述から構造へ、と射程が拡大した。

---

## 次の拡張ロードマップ

### v0.8 候補（短期、1-2週間）
- 新パターン候補のうち優先度「最高」4件を pattern登録
  - **aware-abdication**（最優先：99% の自己警戒）
  - **status-driven-abdication**（algorithmic-abdication の進化的補強）
  - **observer-economy**（時代記述）
  - **critic-trap**（user自身への警鐘）
- physical / linguistic 領域 atom 各3件追加（薄い領域の補強）

### v0.9 候補（中期、1ヶ月）
- 介入 atom 51件のうち高頻度のものを正式登録（counter-pattern 体系化）
- 横断利用の cross-pattern 注釈を全 atom file に追加
- 進化的下地ペアを各 social/cognitive atom file の補足セクションに反映

### v1.0 への道筋（3ヶ月）
- 100 atoms / 30 patterns 分解
- 四層完全マッピング（進化下地 → atom → pattern → 事象）
- 介入 Playbook（壊し方カタログ）の体系化
- atoms-graph の Mermaid自動生成（54 ノード × 関係エッジの可視化）
