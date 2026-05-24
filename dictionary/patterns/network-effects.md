---
id: "network-effects"
name: "ネットワーク効果"
grammar_type: "emergence"
mechanism_id: "E-089"
created: 2026-03-11
---

# network-effects（ネットワーク効果）

参加者の増加に伴い、ネットワーク全体の価値が非線形に増大する構造。

## 定義

ユーザー数や接続数の増加が、既存ユーザーを含む全参加者にとっての価値を高める正のフィードバックループ。臨界量を超えると急速に普及し、支配的地位を獲得する。

## 構造

```
initial_adoption
  → user_value_increase (more users = more value)
    → positive_feedback_loop
      → critical_mass
        → winner-take-most dynamics
```

## 発動条件

1. ユーザー間の相互作用・接続
2. 互換性・標準化
3. 切り替えコストの存在
4. 臨界量への到達

## 失敗条件

- **断片化**: 互換性のない複数ネットワーク
- **鶏と卵**: 初期ユーザー獲得の困難
- **混雑**: ユーザー増加による価値低下
- **マルチホーミング**: 複数ネットワーク並行利用

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | social-media, operating-system |
| economics | marketplace, payment-network |
| politics | voting-bloc, alliance |
| religion | religious-community, pilgrimage-site |
| art | cultural-scene, fan-community |

## 関連パターン

- **scaling**: ネットワーク効果によるスケール拡大
- **standardization**: ネットワーク効果が標準を確立
- **broadcast**: ネットワーク効果が拡散を加速

## メカニズムID

**[NE-01] Direct Network Effects** — ユーザー間直接接続による価値増大
**[NE-02] Indirect Network Effects** — 補完財・サービスを通じた価値増大
