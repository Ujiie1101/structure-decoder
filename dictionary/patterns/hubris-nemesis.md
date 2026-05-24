---
# === Identity ===
slug: "hubris-nemesis"
type: "pattern"

# === Definition ===
name: "傲慢と報復パターン"
formula: "hubris → nemesis → catastrophe"
description: "人間の限界を超えた傲慢（ヒュブリス）が、神々の報復（ネメシス）を招き、破滅に至る。ギリシア悲劇の根本構造。"

# === Composition (atoms) ===
composition:
  - atom: success-blindness
    role: 過去の成功が認知を歪め、傲慢の主観的根拠を作る
  - atom: feedback-suppression
    role: 警告・異論が組織内フィルターで消え、修正機会を奪う
  - atom: scale-mismatch
    role: 行動規模が認知能力を超え、傲慢の客観的破綻条件を作る
composition_formula: "success-blindness × feedback-suppression × scale-mismatch"
composition_note: "主観（自信）×情報（遮断）×客観（能力超過）の積。三者揃ったとき、修正不能なhubrisが固化する。LTCM・Theranos・コダック・ナポレオンのロシア遠征はすべてこの三層が揃った臨界事例。"

# === Components ===
components:
  - name: "hubris"
    description: "傲慢・人間の分を超えた自信"
  - name: "nemesis"
    description: "神罰・報復・均衡の回復"
  - name: "catastrophe"
    description: "破滅・悲劇的結末"

# === Instances ===
instances:
  - entity: "ltcm-collapse"
    layer: "history"
    note: "ノーベル賞受賞者の「市場は数学で支配できる」→46億ドル消失"
  - entity: "theranos"
    layer: "history"
    note: "「一滴の血液で全てを診断」→90億ドルの幻想崩壊"
  - entity: "icarus"
    layer: "religion"
    note: "蝋の翼で太陽に近づく→墜落"

# === Labels ===
labels: ["hubris", "overconfidence", "catastrophe", "nemesis"]

# === Meta ===
updated: 2026-02-17
---

# 傲慢と報復パターン

## 構造式

```
hubris → nemesis → catastrophe
  ↓         ↓          ↓
傲慢      報復       破滅
限界超越   均衡回復    悲劇的結末
```

## 核心

人間が自らの限界を忘れたとき、宇宙の均衡が崩れ、必然的に報復が訪れる。

## 警告サイン

1. 「これまでと違う」という確信
2. 反対意見の排除
3. 成功の内部化（「自分の実力」）
4. 外部環境への鈍感さ

## 適用例

### 哲学

| Entity | Hubris | Nemesis | Catastrophe |
|--------|--------|---------|-------------|
| ピタゴラス | 「万物は数」 | 無理数の発見 | ヒッパソス殺害 |

### 歴史

| Event | Hubris | Nemesis | Catastrophe |
|-------|--------|---------|-------------|
| LTCM | 数学的確信 | ロシア危機 | 46億ドル消失 |
| Theranos | 技術の誇大主張 | SEC調査 | 詐欺で有罪 |
| コダック | 「フィルムに問題ない」 | デジタル化 | 破産 |

## 現代的教訓

- 「絶対に失敗しない」は傲慢の兆候
- 外れ値（Black Swan）への備えの欠如
- 専門家への過信

## 関連パターン

- [[cycle]] - 循環パターン（hubris-nemesisは循環の一部）
- [[transformation]] - 変容パターン
