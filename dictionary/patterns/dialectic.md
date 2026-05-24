---
# === Identity ===
slug: "dialectic"
type: "pattern"

# === Definition ===
name: "弁証法パターン"
formula: "thesis → antithesis → synthesis"
description: "対立を通じた統合の構造。正（テーゼ）と反（アンチテーゼ）の矛盾が、より高次の合（ジンテーゼ）へと止揚される。"

# === Components ===
components:
  - name: "thesis"
    description: "定立・最初の主張"
  - name: "antithesis"
    description: "反定立・否定・矛盾"
  - name: "synthesis"
    description: "綜合・止揚（アウフヘーベン）"

# === Instances ===
instances:
  - entity: "socrates"
    layer: "philosophy"
    note: "問答法（エレンコス）による真理発見"
  - entity: "hegel"
    layer: "philosophy"
    note: "精神の弁証法的自己展開"
  - entity: "marx"
    layer: "philosophy"
    note: "史的唯物論における階級闘争"

# === Labels ===
labels: ["negation", "synthesis", "transformation"]

# === Meta ===
updated: 2026-02-17
---

# 弁証法パターン

## 構造式

```
thesis → antithesis → synthesis
  ↓          ↓           ↓
 正         反          合
 定立       反定立       綜合
```

## 核心

対立は終着点ではなく、より高次の統合への過程である。

## 適用例

### 哲学

| Entity | Thesis | Antithesis | Synthesis |
|--------|--------|------------|-----------|
| ソクラテス | 無知の自覚 | 相手の「知」 | 真理への接近 |
| ヘーゲル | 存在 | 無 | 生成 |
| マルクス | 資本家 | プロレタリア | 共産社会 |

### 歴史

| Event | Thesis | Antithesis | Synthesis |
|-------|--------|------------|-----------|
| フランス革命 | 王政 | 共和制 | ナポレオン体制 |

## 誤用パターン

- antithesisを単なる「反対意見」と解釈
- synthesisを「妥協」と誤解（止揚は両者を超える）
- 静的な三項図式への還元

## 関連パターン

- [[transformation]] - 変容パターン
- [[cycle]] - 循環パターン
