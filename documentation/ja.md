<!-- ELUCENIA technical documentation · isth-cid · ja · no clinical/professional/rights approval -->

# ISTH顕性播種性血管内凝固スコア

[条件・出典・許諾](https://elucenia.org/ja/tools/isth-cid)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 血小板

`plaq`

- `0` — \> 100000/µL
- `1` — 50.000 ～ 100.000 /µL
- `2` — \< 50000/µL

### フィブリンマーカー（DダイマーまたはFDP）

`dd`

- `0` — 上昇なし
- `2` — 中等度上昇
- `3` — 著しい増加

### プロトロンビン時間延長

`tp`

- `0` — \< 3 s
- `1` — 3 ～ 6 s
- `2` — \> 6 s

### フィブリノゲン

`fib`

- `0` — ≥ 1 g/L
- `1` — \< 1 g/L (100 mg/dL)

## 方法の版

ISTH/Taylor 2001：顕性DIC，血小板/FDP/PT/フィブリノゲン，合計0–8

## 記載された計算式

血小板\>100千は0，50–100千は1，\<50千は2 · Dダイマー/FDP上昇なし0，中等度2，著明3 · PT延長\<3 sは0，3–6 sは1，\>6 sは2 · フィブリノゲン≥1 g/Lは0，\<1 g/Lは1。最大：8。

前提：DICに関連する基礎疾患（敗血症，外傷，がん，産科合併症など）。

## 限界・対象集団

播種性血管内凝固（DIC）に合致する基礎疾患がある状況で、臨床データと検査データを組み合わせて適用します。過程は動的であり、評価の反復が必要です。スコアだけでは診断は証明されず、精度は対象集団と点数の層によって異なります。

## 参考文献

- [Taylor FB Jr et al. Towards definition, clinical and laboratory criteria, and a scoring system for disseminated intravascular coagulation. Thromb Haemost, 2001.](https://doi.org/10.1055/s-0037-1616068)

- [Levi M et al. Guidelines for the diagnosis and management of disseminated intravascular coagulation. Br J Haematol, 2009.](https://doi.org/10.1111/j.1365-2141.2009.07600.x)

- [Larsen JB et al. Disseminated intravascular coagulation diagnosis: Positive predictive value of the ISTH score in a Danish population. Research and Practice in Thrombosis and Haemostasis, 2021. Table 1 (fibrinogen boundary).](https://doi.org/10.1002/rth2.12636)

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
