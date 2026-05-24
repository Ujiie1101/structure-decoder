---
id: "incentive-distortion"
name: "インセンティブ歪曲"
grammar_type: "emergence"
mechanism_id: "E-066"
created: 2026-03-11
---

# incentive-distortion（インセンティブ歪曲）

制度設計が意図せぬ行動を誘発し、当初の目的を損なう構造。

## 定義

報酬・罰則・規制などのインセンティブ設計が、設計者の意図とは異なる行動（gaming, 抜け穴利用, 数字の操作）を合理的に引き起こし、制度の実効性を蝕む。

## 構造

```
incentive_design
  → agents_optimize_to_measured_metric
    → divergence_from_intended_outcome
      → gaming_and_exploitation
        → institutional_failure
```

## 発動条件

1. 測定可能な指標への報酬紐付け
2. 指標と真の目的の乖離（Goodhart's Law）
3. 合理的エージェント
4. 監視・執行コストの存在

## 典型的形態

- **Cobra Effect**: 報奨が問題を悪化させる
- **Campbell's Law**: 測定指標が目標になると腐敗する
- **Teaching to the Test**: 指標最適化が本質を空洞化
- **Creative Compliance**: 形式遵守と実質回避

## 適用事例

| Layer | Entities |
|-------|----------|
| economics | executive-compensation, subprime-crisis |
| politics | gdp-obsession, kpi-culture |
| technology | engagement-metrics, click-bait |
| history | soviet-planning, vietnam-body-count |

## 関連パターン

- **principal-agent-divergence**: 情報非対称下での歪曲
- **penalty-as-license**: 罰則がコストとして計算される
- **regulatory-lag**: 規制の抜け穴利用

## 注意

「測定されるものは改善される」の暗い側面。数字は操作され、指標は空洞化し、制度は形骸化する。設計者の合理性が、被設計者の合理性に敗北する。
