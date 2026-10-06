<!-- ELUCENIA technical documentation · bisap · ja · no clinical/professional/rights approval -->

# BISAPスコア

[条件・出典・許諾](https://elucenia.org/ja/tools/bisap)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 尿素 \> 53 mg/dL（BUN \> 25 mg/dL）

`bun`

### 精神状態の変化（Glasgow \< 15）

`mental`

### SIRS（2項目以上）

`sirs`

### 年齢 \> 60 歳

`idade`

### 画像上の胸水

`derrame`

## 方法の版

BISAP/Wu 2008：5因子、最初24 h、BUN \>25 mg/dL、年齢\>60

## 記載された計算式

最初24時間で各1点：BUN \>25 mg/dL（尿素\>53 mg/dL）、I意識障害、SIRS、A年齢\>60歳、P胸水。

SIRS：体温\<36または\>38 °C、心拍\>90 bpm、呼吸\>20回/分またはPaCO₂ \<32 mmHg、白血球\<4000または\>12000/mm³または桿状核\>10%のうち≥2。

## 限界・対象集団

2008年のBISAPは、急性膵炎の最初の24時間のデータを使い、院内死亡のリスクを層別化します。BUN\>25 mg/dLと年齢\>60歳はスコア項目であり、最低限の組入れ基準ではありません。壊死、臓器不全の評価とサブグループへの適用可能性は、それぞれの出典に依存します。観察された率は、個人の予後を確実に示すものではありません。

## 参考文献

- [Wu BU et al. The early prediction of mortality in acute pancreatitis: a large population-based study. Gut, 2008.](https://doi.org/10.1136/gut.2008.152702)

- [Singh VK et al. A prospective evaluation of the bedside index for severity in acute pancreatitis score in assessing mortality and intermediate markers of severity in acute pancreatitis. Am J Gastroenterol, 2009.](https://doi.org/10.1038/ajg.2009.28)

- [Banks PA et al. Classification of acute pancreatitis—2012: revision of the Atlanta classification and definitions by international consensus. Gut, 2013.](https://doi.org/10.1136/gutjnl-2012-302779)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

BISAP 0から2: 死亡リスクが低い

導出低リスク群では死亡率1%未満。最初の48 hは臨床的再評価を維持する。


### 2

BISAP ≥ 3: 死亡および合併症のリスク増加

臓器不全（OR 7,4）、持続性不全（OR 12,7）および膵壊死（OR 3,8）と関連；ICUまたは中間ケア病棟を検討する。

