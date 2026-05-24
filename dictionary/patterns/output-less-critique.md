---
id: "output-less-critique"
name: "消費型批判"
grammar_type: "fragmentation"
mechanism_id: "F-010"
created: 2026-03-15
composition:
  - atom: alternative-cost
    role: 代案を作る思考・実装コストが批判コストより圧倒的に高い
  - atom: empathy-incentive
    role: 共感を獲得する社会報酬が批判発話に偏って配分される
  - atom: stake-free-visibility
    role: 賭けなしに目立てる構造（匿名性、リプライ拡散）
composition_formula: "alternative-cost × empathy-incentive × stake-free-visibility"
composition_note: "経済（コスト非対称） × 報酬（共感偏重） × 構造（賭けなき可視性）の三層。SNS時代以前から存在した構造だが、stake-free-visibility が劇的に強化されたことで、現代特有の規模になった。介入は3つすべてに同時に手をつける必要がある（代案義務化＋報酬構造の再設計＋身元紐付け）。"
---

# output-less-critique（消費型批判）

代案なき批判が、エネルギーを消費するだけで何も生まない構造。

## 定義

感情の発散と共感の獲得で完結し、問題解決や改善という「出力」を生まない批判行為。フィードバック・ループが断絶した状態。

## 構造

```
problem_perception
  → emotional_reaction
    → expression_of_dissatisfaction
      → social_validation (likes, retweets)
        → energy_exhaustion
          → no_output (loop terminates)
```

## 発動条件

1. 代案を考えるコストの回避
2. 共感獲得のインセンティブ（SNSアルゴリズム）
3. 責任回避（代案を出すとリスクが生じる）
4. 「批判している」という自己満足

## 失敗条件（建設的批判への転換）

- **代案の義務化**: 問題指摘と同時に代案を示す
- **具体的解像度**: 抽象的な批判を許さない
- **出力の定義**: この批判で何が変わるかを問う
- **相手視点の想像**: 批判対象の立場で考える

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | sns-outrage-cycle, twitter-pile-on |
| politics | partisan-criticism, media-criticism |
| economics | consumer-complaint-without-action |
| philosophy | nihilistic-critique |

## 関連パターン

- **feedback**: 消費型批判はフィードバックの断絶形態
- **fragmentation**: 消費型批判が内部分裂を加速
- **amplification**: SNSが消費型批判を増幅

## 出典記事

`200_Output/20260315_criticism-literacy-yamaguchi-shu.md`

## メカニズムID

**[F-03] Sectarian Split** — 批判が分断を生み、分断がさらなる批判を生む
