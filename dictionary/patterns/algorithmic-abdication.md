---
id: "algorithmic-abdication"
name: "アルゴリズム放棄"
alias: "Algorithmic Abdication"
grammar_type: "emergence"
mechanism_id: "E-145"
created: 2026-04-29
source: Day65記事 / atoms-graph.md（v0.2）
related:
  - decision-delegation-desire（DDD-01、上流の心理パターン）
  - judgment-evaporation（個人スケール版、Day64）
  - principal-agent-divergence
  - automation
  - bystander-economics
composition:
  - atom: scale-mismatch
    role: 規模が認知能力を超える（客観条件）
  - atom: responsibility-aversion
    role: 担当者が結果責任を回避する（動機）
  - atom: complexity-overwhelm
    role: 処理すべき変数が許容を超える（認知負荷）
  - atom: authority-availability
    role: AI が受け皿として利用可能（供給条件）
composition_formula: "scale-mismatch × responsibility-aversion × complexity-overwhelm × authority-availability"
composition_note: "decision-delegation-desire の3atomに scale-mismatch を加えた4-atom構成。前3者は人間心理・制度・認知の常在条件、scale-mismatch は組織が認知能力を超えた瞬間に発火する。AIは前3者すべてに最適化された受け皿として登場し、4-atom揃った瞬間に組織は判断を構造的に手放す。"
---

# algorithmic-abdication（アルゴリズム放棄）

組織が判断を AI/アルゴリズムに**構造的に**手放す現象。意図ではなく圧力で進行する。

## 定義

組織が直面する案件規模・判断複雑性・責任回避欲求・受け皿供給の **4つの圧力**が同時に揃ったとき、判断主体が組織から消滅し、アルゴリズムへの依存が「合理的選択」として制度化される構造。

decision-delegation-desire の組織スケール拡張形。個人レベルの委託欲求が、組織レベルでは scale-mismatch を加えた4-atom構成として顕在化する。

## 公式

```
algorithmic-abdication
  = scale-mismatch          （規模が認知を超える）
  × responsibility-aversion （結果責任を負いたくない）
  × complexity-overwhelm    （変数が処理能力を超える）
  × authority-availability  （AIが受け皿として用意されている）
```

4つすべて揃ったとき発動。1つでも欠ければ放棄は完成しない。

## 発動条件

1. **規模超過**: 案件処理数が個別判断の認知容量を超える
2. **責任構造の偏り**: 担当者の評価が「決断の結果」中心、「決断しなかったこと」を評価しない制度
3. **多変数性**: 各案件で評価すべき軸が10以上になる
4. **AI受け皿の整備**: 業界向け AI ソリューションが商用化済み

4つ揃わない場合の停止形態:
- scale-mismatch のみ欠如 → 担当者の手作業継続（過労状態）
- responsibility-aversion のみ欠如 → 担当者が個人責任で判断（古典的判断組織）
- complexity-overwhelm のみ欠如 → 単純基準での自動化（古典的automation）
- authority-availability のみ欠如 → コンサル・専門家委員会での代替

## 失敗条件（abdicationが回避される条件）

### 個別原子への介入
- **scale-mismatch**: トリアージ導入、サービスレベル制限、規模縮小
- **responsibility-aversion**: 「AI判定を採用した」担当者の署名強制、評価制度の改革
- **complexity-overwhelm**: 判断軸の意図的縮減、3軸圧縮
- **authority-availability**: 受け皿の競合化、複数AI並立、不一致の可視化

### 組み合わせ介入（最強）
**responsibility-aversion × authority-availability への同時介入** = 「判定者の署名」+「受け皿の競合化」。4原子のうち2原子を同時に弱める。

## 判別法

1. 担当者の発話に「システムが」「AIが」「アルゴリズムが」が頻出する
2. 案件処理数が、担当者数 × 個別判断容量を超えている
3. 評価制度に「決断しなかったこと」を測る指標がない
4. 業界標準のAIソリューションに依存している

4つ揃うと algorithmic-abdication が作動している。

## 適用事例

| 業界 | 主要事例 | 表面 | abdicationの現場 |
|------|---------|------|---|
| 福祉 | Robodebt（豪、2016-2019） | AI債務回収 | 担当者が「システムフラグ」を確認するだけ／46万件の不当請求 |
| 福祉 | SyRI（蘭、2014-2020） | 不正受給予測AI | 違法判決（2020）／アルゴリズムが特定地域住民を標的 |
| 採用 | HireVue（米、2014-2021） | AI面接表情分析 | 科学的根拠なしと批判→機能撤回（2021） |
| 採用 | Amazon採用AI（2018） | 履歴書スクリーニング | 女性差別を学習→運用停止 |
| 司法 | COMPAS（米、2010s-） | 再犯予測 | ProPublica調査で人種偏向（2016） |
| 教育 | A-level algorithm（英、2020） | コロナ下の入試判定 | 撤回騒動／格差再生産 |

## 関連パターン

- **decision-delegation-desire (DDD-01)**: 個人スケールの上流パターン。算術的に scale-mismatch を加えると本パターン
- **judgment-evaporation**: 個人スケールでの判断主体消失。本パターンの個人版
- **principal-agent-divergence**: 古典的代理人理論。AI受け皿の場合に射程外
- **automation**: 自動化一般。判断責任の蒸発までは射程外
- **bystander-economics**: 「誰も責任を負わない」状態の経済学的同型
- **mission-drift**: 同じ「組織の漸進的逸脱」だが、漂流先が AI ではなく KPI
- **groupthink**: 組織内合意形成の失敗。本パターンと並行発動しうる

## 哲学的親族

- **マックス・ヴェーバー『支配の社会学』(1922)**: 鉄の檻。本パターンはその AI 時代版
- **ハンナ・アーレント『精神の生活』(1978)**: 思考と判断の分離。本パターンは判断の組織的撤退
- **エーリッヒ・フロム『自由からの逃走』(1941)**: 自由の重荷。本パターンの心理的根源
- **Lisanne Bainbridge "Ironies of Automation" (1983)**: 自動化逆説の古典

## 出典記事

`200_Output/100-day-kos/day-065-algorithmic-abdication.md`

## 核心洞察

> **AIガバナンスでは止まらない。4つの原子それぞれの時間軸に手を伸ばす必要がある。**
>
> scale-mismatch は進化的、responsibility-aversion は組織論的、complexity-overwhelm は社会学的、authority-availability は技術史的。4つの長い時間軸が2020年代に**収束**した場所に、algorithmic-abdication が出現した。

## メタ観察

本パターンは **Knowledge OS の atoms層**から派生した最初の登録パターン。

通常パターンは事象観察から発見される。本パターンは逆に、**21 atoms の未試行組み合わせから推論**された後、既存事象（Robodebt, SyRI, COMPAS）にマッチして登録された。

これは atoms層の検証実験：「atom組み合わせから新パターンが演繹可能か」という問いに対する yes の証拠となる。

## 反証条件

4つの原子のうち1つでも欠けている組織で algorithmic-abdication が観察された場合、本パターンの定義は再検討が必要。

観察期間：2026年Q3〜Q4。検証対象：豪・蘭・英・米の関連政策動向。
