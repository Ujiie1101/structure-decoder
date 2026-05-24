---
id: "information-asymmetry"
name: "情報非対称"
grammar_type: "emergence"
mechanism_id: "E-070"
created: 2026-03-11
---

# information-asymmetry（情報非対称）

取引当事者間の情報格差が市場を歪め、非効率や市場崩壊を引き起こす構造。

## 定義

一方の当事者が他方より多くの情報を持つとき、情報劣位者は逆選択やモラルハザードのリスクに直面し、市場メカニズムが機能不全に陥る。

## 構造

```
information_gap_between_parties
  → adverse_selection (ex ante)
    → good_quality_exits_market
      → market_unraveling
  → moral_hazard (ex post)
    → hidden_action_exploitation
      → contract_failure
```

## 二つの形態

### 逆選択（Adverse Selection）

- **時点**: 契約前
- **問題**: 隠れた属性
- **例**: レモン市場、保険の高リスク者集中

### モラルハザード（Moral Hazard）

- **時点**: 契約後
- **問題**: 隠れた行動
- **例**: 保険加入後の注意低下、救済期待のリスクテイク

## 発動条件

1. 情報の私的性質（観察不能・検証不能）
2. 情報獲得コストの非対称
3. シグナリング/スクリーニングの不完全性
4. 強制開示制度の欠如

## 適用事例

| Layer | Entities |
|-------|----------|
| economics | akerlof-lemons, insurance-market, credit-market |
| technology | platform-trust, online-marketplace |
| politics | lobbying, regulatory-capture |
| history | subprime-crisis, enron |

## 関連パターン

- **principal-agent-divergence**: 情報非対称の典型的文脈
- **incentive-distortion**: 情報格差下でのインセンティブ設計
- **invisible-hand**: 情報非対称が見えざる手を阻害

## 注意

完全情報の仮定が崩れるとき、市場は「見えざる手」から「見えない罠」に変わる。Akerlof, Spence, Stiglitzの情報経済学が解明した市場の暗部。
