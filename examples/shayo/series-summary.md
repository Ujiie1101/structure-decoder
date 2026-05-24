---
id: "shayo-series-summary"
book: "斜陽"
author: "太宰治"
year: 1947
type: "series-summary"
created: 2026-05-13
total_chapters: 8
status: "completed"
---

# 『斜陽』_読み直し ── シリーズ完結報告

## 全章スコア

| 章 | スコア | テーマ |
|---|---|---|
| 第一章 | 91 | 徴候の登記（蛇、地理的没落） |
| 第二章 | 92 | 事件の実現（火事、生気の入れ替わり） |
| 第三章 | 91 | 過去の侵入（編物、夕顔日誌、6年前） |
| 第四章 | 92 | 書字の事件（三通の手紙） |
| 第五章 | 93 | 消失と誕生の同時性（母の死、革命家宣言） |
| 第六章 | 92 | 戦闘と幻滅の同時性（上京、屈辱、自殺予告） |
| 第七章 | 93 | 直治の遺書（貴族の引き受け） |
| 第八章 | 93 | 最終手紙（斜陽から太陽への反転） |

平均：92.0 / 全章 threshold 90 以上達成

## 章末の言葉の系列

| 章 | 章末 |
|---|---|
| 1 | （胸の中の蛇） |
| 2 | 「私たちの本当の地獄がはじまった」 |
| 3 | 「不良とは、優しさの事ではないかしら」 |
| 4 | 「マイ、チャイルド」 |
| 5 | 「ピエタのマリヤ」 |
| 6 | 「弟の直治は、その朝に自殺していた」 |
| 7 | 「僕は、貴族です」 |
| 8 | 「マイ、コメデアン。昭和二十二年二月七日」 |

## 第四章＝第七章の対称（書字の章）

| 比較項目 | 第四章 | 第七章 |
|---|---|---|
| 書き手 | かず子 | 直治 |
| 宛先 | 上原 | かず子 |
| 通数 | 三通 | 一通 |
| 主題 | 押しかけ愛人志願 | 自殺の説明 |
| 結末 | 「マイ、チャイルド」 | 「僕は、貴族です」 |
| 結末の効果 | 宛先の事後変動 | 出自の最後の引き受け |

## 太宰の手つきの章別総覧

- 第一章：地の文（徴候の登記）
- 第二章：地の文＋直接話法（事件と村の応答）
- 第三章：地の文＋夕顔日誌引用（過去の螺旋運動）
- 第四章：手紙のみ（読者の立ち位置を動かす）
- 第五章：地の文＋夢（同じ記号で二つの事件を結合）
- 第六章：地の文＋直接話法（一行で章全体を裏返す）
- 第七章：遺書のみ（章全体を事件の内容の事後開封）
- 第八章：最終手紙のみ＋日付（書名そのものを反転）

## シリーズ全体の構造原理

1. **徴候の長距離回収**: 第一章の蛇が第五章で母を取り、第八章で記号系列が完結
2. **書字の章の対称配置**: 第四章（かず子の手紙）と第七章（直治の遺書）が鏡像をなす
3. **過去の螺旋運動**: 第三章で過去が侵入し、章を進めるごとに過去の事件が重ねられる
4. **章末による物語の重力反転**: 各章末で次章の方向を決める一行が置かれる
5. **書名そのものの反転**: 「斜陽」が最終章で「太陽」に書き換えられる

## 集約された新造語（53件）

`.neologism-buffer.json` を参照。

内訳：
- atom候補：27件
- pattern候補：26件
- meta候補（book-decompose方法論レベル）：2件

## Phase 3：KOS バッチ昇格結果（2026-05-13）

53件のうち**13件**を Knowledge OS に投入。残り40件は `.neologism-buffer.json` に保留。

### 投入 atom 8件

| Atom | 章 | Domain |
|---|---|---|
| sign-long-distance-recovery（徴候の長距離回収）| 1→5→8 | linguistic |
| writing-irreversibility（書字の不可逆性）| 4 | linguistic |
| addressee-postvariation（宛先の事後変動）| 4 | linguistic |
| spiral-of-past（過去の螺旋運動）| 3 | cognitive |
| inheritance-unidirectionality（継承の片道性）| 1 | social |
| family-vitality-conservation（家族の生気保存則）| 2 | social |
| deviant-tenderness（逸脱者の優しさ）| 3 | social |
| retroactive-origin-acceptance（出自の事後引き受け）| 7 | cognitive |

### 投入 pattern 5件

| Pattern | 章 | Composition |
|---|---|---|
| disappearance-emergence-synchrony（消失と誕生の同時性）| 5 | inheritance-unidirectionality × sign-long-distance-recovery × family-vitality-conservation |
| delayed-delivery-as-education（遅延配達としての教育）| 3 | spiral-of-past × generational-amnesia × sign-long-distance-recovery |
| simultaneous-contradiction-operation（矛盾の同時運用）| 4 | writing-irreversibility × addressee-postvariation × confession-mimicry |
| tragedy-to-comedy-dispatch（悲劇から喜劇への送り出し）| 8 | retroactive-origin-acceptance × writing-irreversibility × inversion |
| pseudo-thought-from-bar（酒場由来の疑似思想）| 7 | borrowed-pedigree × confession-mimicry × deviant-tenderness |

### 投入 meta-atom 2件（135_Meta/book-level-techniques/）

| Meta-Atom | 章 | 内容 |
|---|---|---|
| chapter-pivot-line（章を裏返す一行）| 6 | 章末の一行で章全体の意味を後付け反転する技法 |
| title-self-inversion（書名の自己反転）| 8 | 書名と内容の関係を終端で反転する技法 |

book-level スケールの操作技法として、event-level の通常atomと別レイヤーに登録。

### 保留（38件）

- 既存 success-blindness と重複する「自己疑問の欠如としての成功」など 1件は supersededとして見送り
- 残り37件は今後の atom-decompose / kos-promote セッションで個別検討

## 関連ファイル

- 全章 source: `chapter-N-source.md`（N=1..8）
- 全章 Mode 5 reading-note: `chapter-N-reading-note.md`（N=1..8）
- 全章 Mode 6 published: `published/chapter-N.md`（N=1..8）
- 造語バッファ: `.neologism-buffer.json`
- 進捗状態: `.book-series-state.json`
- KOS投入先: `130_Structure/atoms/` および `130_Structure/patterns/`
