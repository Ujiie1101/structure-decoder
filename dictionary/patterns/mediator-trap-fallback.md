---
id: "mediator-trap-fallback"
name: "仲裁者の罠"
grammar_type: "emergence"
created: 2026-05-13
source_work: "夏目漱石『坊っちゃん』第十章（祝勝会の喧嘩を仲裁しようとした坊っちゃんと山嵐だけが警察に連れていかれる）"
composition:
  - atom: frontal-method-purity
    role: 仲裁者が現場に残る理由
  - atom: responsibility-aversion
    role: 当事者は逃げる
---

# mediator-trap-fallback（仲裁者の罠）

喧嘩・対立・不正を**止めようとした者だけが残り、罰せられる**装置。当事者は退却し、現場の制度的処理（警察・人事・裁判）は仲裁者を「現場に居た者」として処理する。

## 定義

時系列構造:

1. **対立発生**: AとBが対立する
2. **仲裁者参入**: 第三者Cが止めに入る
3. **両側からの反発**: AとBが一時的に共通の敵Cを見つける
4. **制度的処理の到着**: 警察・人事などが介入
5. **当事者退却**: AとBは逃げる
6. **仲裁者単独で残留**: Cだけが現場に残る
7. **誤った帰責**: 制度はCを「現場の主体」として処理する

「誰が原因か」ではなく「誰が現場にいるか」で罰が決まる。

## 構造

```
conflict_emerges（対立発生）
  → mediator_enters（仲裁者参入）
    → common_enemy_formation（両側が共通の敵に）
      → institutional_arrival（制度的処理の到着）
        → perpetrators_flee（当事者退却）
          → mediator_remains（仲裁者残留）
            → wrong_attribution（誤帰責）
```

## 観察可能な現代具体例

- 組織の不正を内部告発した人物が「組織の信頼を傷つけた」として処分される
- SNSで加害者の身元を特定した人物が、プライバシー侵害で訴えられる
- ハラスメントを止めようとした第三者が、自身の管理責任を問われる
- 喧嘩を止めに入った野次馬が暴行罪で立件される

## 対抗装置

- 仲裁者が**自分の立ち位置を即座に書面化**する（警察到着前に身分・目的を明示）
- 仲裁の前に当事者の氏名と所属を控える
- 単独で介入しない（複数仲裁者＋第三者証言）
- 制度的処理が来る前に退却する判断

## 関連パターン

- [bystander-economics](bystander-economics.md) — 傍観の経済学との対比（こちらは仲裁の経済学）
- [un-accusable-attack](un-accusable-attack.md) — 制度的版
- [responsibility-aversion] (atom) — 当事者退却の駆動力
