---
id: "prevention-invisibility"
name: "予防の不可視性"
type: "atom"
domain: "cognitive"
created: 2026-04-29
---

# 予防の不可視性

「**防いだ被害**」が認知も評価もできない構造。発生した被害は数えられるが、未然に防いだ被害は反実仮想でしか語れず、データとして残らない。

## 起源（Why this exists）

人間の認知は事象（変化）を検知するように進化しており、**非事象（防がれたもの）**を検知できない。何も起きなかった日は記憶されない。事故は記憶されるが、事故が起きなかった日は記憶されない。

加えて、評価制度・予算配分・組織評価は通常、**測定可能な指標**で構築される。発生した被害は測定できる（件数・損失額）。防いだ被害は測定不能（反実仮想・推計）。結果として、予防業務は構造的に過小評価される。

これは [visibility-asymmetry]（既存）の特殊形だが、独立した atom として扱う。なぜなら、ここで対象になっているのは「**反事実そのものの不可視性**」だから。

## 観察可能なproxy

- 予防部門と事後対応部門の予算比較
- 「今四半期、何件防ぎましたか？」への答えの困難
- セキュリティ・安全・コンプライアンス部門の評価軸
- 「事故ゼロ」が評価される vs 「無能」と見なされる二極

## 介入点（Disable conditions）

- 反実仮想の数値化（推計手法の導入）
- 業界・歴史的ベンチマークとの比較（相対評価）
- 予防成果の物語化（「もしもこれがなかったら」を語る）
- 予防部門の独立予算化（事後対応部門と分離）

## 関与パターン

- [bystander-economics](../patterns/bystander-economics.md) — ベネフィット側の不可視性
- [prevention-self-erasure](../patterns/prevention-self-erasure.md) — 予防の自己消去（基底層として作動、composition の主軸）
- [epidemiological-amnesia](../patterns/epidemiological-amnesia.md) — 公衆衛生領域での自己消去
- （拡張候補: visibility-asymmetry, measurable-displacement, goodharts-law）

## 補足

[visibility-asymmetry]（既存、causal-misattribution で使用）との違い:
- **visibility-asymmetry**: 見える事象 vs 見えない構造
- **prevention-invisibility**: 起きた事象 vs 起きなかった事象（反実仮想）

前者は同時並存する2要素の見え方の差、後者は時間軸での起きた／起きなかったの非対称。

bystander-economics の中で、prevention-invisibility は**便益側の盲目**として作動する。傍観のコストは見えず（[action-cost-asymmetry]）、行動の便益も見えない（prevention-invisibility）。両側からの非対称が傍観を最適戦略に固定する。

## Self-erasure through success（成功による自己消去）

予防が高度に機能した場合、それは自分自身の必要性の証拠を消去する。被害が発生しなければ「予防が要らなかった」と区別できないからである。

これは prevention-invisibility の時間軸での先鋭化形：
- 短期：今四半期の防いだ被害が測定できない（基本構造）
- 長期：60年機能した予防が「そもそも要らなかった」と再解釈される（self-erasure）

長期形では、便益（不可視）とコスト（可視）の非対称が、世代を超えて累積する。便益を経験した世代が退場し、コストだけが日常に残ると、予防そのものが「過剰反応」「歴史の遺物」として再フレーミングされる。

[experiential-amnesia](experiential-amnesia.md) と連動：身体化された記憶を持つ世代が退場するか、記憶が「他人事化」した瞬間、self-erasure が完成する。

## 事例

- **ビタミンK拒否（2026, 米）**: 1961年から60年機能した新生児ビタミンK注射により、頭蓋内出血で死ぬ赤ちゃんがほぼ消えた。結果、現代の親が「死の証拠」を見たことがなくなり、注射の必要性が想像できなくなった。CNN 2026-05-08 報道で新生児出血死が再発。`200_Output/substack-daily/2026-05-11-prevention-self-erasure.md` で扱う。
- **公衆衛生インフラ全般（コレラ・はしか・結核）**: 同型構造。便益が成功するほど、便益の必要性が見えなくなる。
- **対テロ・対サイバー攻撃**: 防がれたインシデントが「過剰投資」として攻撃される構造。
