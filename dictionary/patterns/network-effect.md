---
id: "network-effect"
name: "ネットワーク効果"
grammar_type: "emergence"
mechanism_id: "E-088"
created: 2026-03-11
---

# network-effect（ネットワーク効果）

利用者が増えるほど、各利用者にとっての価値が増大する構造。

## 定義

ネットワークへの参加者数がそのネットワークの価値を決定する。メトカーフの法則（価値 ∝ n²）に従い、臨界質量を超えると爆発的成長と独占が生じる。直接効果（同種ユーザー間）と間接効果（補完財）の二類型。

## 構造

```
initial_users (n)
  → value_increase (∝ n or n²)
    → more_users_attracted
      → positive_feedback_loop
        → winner-take-all / lock-in
```

## 発動条件

1. ユーザー間相互作用がある
2. 参加コストより参加便益が大きい
3. 互換性・標準化がある
4. 臨界質量（クリティカルマス）到達

## 失敗条件

- **分断**: 互換性のない複数ネットワーク
- **負の外部性**: 混雑・スパム・質の低下
- **代替出現**: より優れたネットワークへの移行
- **規制介入**: 独占解体・相互接続義務

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | facebook, telephone, fax, windows, visa |
| economics | stock-exchange, language, currency |
| history | silk-road, roman-roads |
| philosophy | lingua-franca, academic-network |
| art | hollywood, art-market |

## 関連パターン

- **emergence**: ネットワーク効果は創発の一形態
- **cascade**: ネットワーク内での連鎖
- **substitution**: ネットワーク間の置換
- **constraint**: ロックイン効果による制約

## メカニズムID

**[E-03] Network Externality** — 正の外部性による収穫逓増
