---
id: "abstraction"
name: "抽象化"
grammar_type: "emergence"
mechanism_id: "E-005"
layer: 3
domains: ["technology"]
created: 2026-03-11
---

# abstraction（抽象化）

具体的詳細を隠蔽し、本質的構造を抽出することで、複雑性を管理可能にする構造。

## 定義

実装詳細から独立したインターフェースを提供し、異なる具体を同一の抽象として扱う。レイヤー化、モジュール化、概念化の基盤。複雑性の封じ込めと、汎用性の獲得を両立。

## 構造

```
concrete_complexity
  → essential_extraction
    → interface_definition
      → implementation_hiding
        → generalization / reusability
```

## 発動条件

1. 複雑性の存在
2. 本質/偶有の区別可能性
3. インターフェース設計
4. 抽象化コストの許容

## 失敗条件

- **漏れのある抽象化**: 詳細が漏出
- **過剰抽象化**: 具体性の喪失
- **性能劣化**: 抽象化オーバーヘッド
- **誤った本質**: 本質抽出の失敗

## 適用事例

| Layer | Entities |
|-------|----------|
| technology | api, virtual-machine, programming-language, cloud |
| philosophy | platonic-forms, universals, essence |
| art | abstract-art, minimalism |
| economics | money, derivative, index |
| mathematics | set-theory, category-theory |

## 関連パターン

- **emergence**: 抽象化からの新概念創発
- **scaling**: 抽象化によるスケール可能性
- **substitution**: 抽象化による実装置換
- **standardization**: 抽象化と標準化
