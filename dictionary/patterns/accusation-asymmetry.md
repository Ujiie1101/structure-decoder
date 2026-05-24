---
id: "accusation-asymmetry"
name: "告発の非対称"
grammar_type: "emergence"
created: 2026-05-13
source_work: "夏目漱石『坊っちゃん』第十一章（杉並木で殴られた赤シャツが警察に届けない── 届ければ芸者と泊まったことが公的記録に残るから）"
composition:
  - atom: stake-free-visibility
    role: 被害者は被害を隠す必要がない
  - atom: face-investment
    role: 加害者は自分の加害を公開できない
---

# accusation-asymmetry（告発の非対称）

告発の権利は両側にあるが、**加害者は告発できない、被害者は告発できる**という非対称。加害を告発するためには、加害を公開する必要があるから。

## 定義

二項構造:

1. **被害者側**: 被害を公開しても自分の損失は増えない（被害は隠す必要がない）
2. **加害者側**: 加害を告発するには、加害行為そのものを公開しなければならない

このため、加害者は私的制裁を受けても**法的告発に踏み切れない**。加害者の沈黙が、私的告発（内部告発・暴露・直接対峙）の成立条件になる。

## 構造

```
private_sanction（私的制裁）
  → asymmetric_publication_cost
    ├─ victim_side: low cost to publicize（被害公開コスト低）
    └─ perpetrator_side: high cost to publicize（加害公開コスト高）
      → perpetrator_silence（加害者沈黙）
        → space_for_private_justice（私的正義の射程確保）
```

## 観察可能な現代具体例

- MeToo運動で加害者が法的措置を取れない
- 企業のハラスメント加害者が反訴を躊躇する
- 不倫の証拠を握られた政治家が告発できない
- 横領の現場を見られた管理職が窃盗者を告発できない
- セクハラ加害者が「名誉毀損」を訴えにくい

## 関連条件

非対称が成立する条件:
- 加害行為が**告発時に追加開示される**情報を含む
- 加害者側が**社会的地位・信用に依存**している
- 被害者側に**失うものが相対的に少ない**

これらが揃わないと、非対称は消える（加害者も告発に踏み切る）。

## 対抗装置（加害者側から見た強化）

加害者が告発の非対称を克服したい場合:
- 加害事実を**先に**自分で公開する（先制告白）
- 加害事実と告発内容を分離する技術（弁護士介在）

## 関連パターン

- [un-accusable-attack](un-accusable-attack.md) — 対の構造
- [hubris-nemesis](hubris-nemesis.md) — 加害者の没落構造
- [self-undermining-success](self-undermining-success.md) — 加害者の自滅構造
