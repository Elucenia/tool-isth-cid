<!-- ELUCENIA technical documentation · isth-cid · zh · no clinical/professional/rights approval -->

# ISTH 显性弥散性血管内凝血评分

[条件、来源与许可](https://elucenia.org/zh/tools/isth-cid)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 血小板

`plaq`

- `0` — \> 100000/µL
- `1` — 50.000 至 100.000 /µL
- `2` — \< 50000/µL

### 纤维蛋白标志物（D-二聚体或纤维蛋白降解产物）

`dd`

- `0` — 无升高
- `2` — 中度升高
- `3` — 明显增加

### 凝血酶原时间延长

`tp`

- `0` — \< 3 s
- `1` — 3 至 6 s
- `2` — \> 6 s

### 纤维蛋白原

`fib`

- `0` — ≥ 1 g/L
- `1` — \< 1 g/L (100 mg/dL)

## 方法版本

ISTH/Taylor 2001：显性DIC，血小板/FDP/PT/纤维蛋白原，总计0–8

## 已记录的公式

血小板\>100千计0，50–100千计1，\<50千计2 · D-二聚体/FDP无升高0、中度2、显著3 · PT延长\<3 s计0，3–6 s计1，\>6 s计2 · 纤维蛋白原≥1 g/L计0，\<1 g/L计1。最高：8。

前提：存在DIC相关基础疾病（脓毒症、创伤、癌症、产科并发症等）。

## 限制与适用人群

应在基础疾病与弥散性血管内凝血（DIC）相符的情境下应用，结合临床和实验室数据。病程是动态的，需要重复评估。评分本身不能证实诊断；准确性因人群及评分分层而异。

## 参考文献

- [Taylor FB Jr et al. Towards definition, clinical and laboratory criteria, and a scoring system for disseminated intravascular coagulation. Thromb Haemost, 2001.](https://doi.org/10.1055/s-0037-1616068)

- [Levi M et al. Guidelines for the diagnosis and management of disseminated intravascular coagulation. Br J Haematol, 2009.](https://doi.org/10.1111/j.1365-2141.2009.07600.x)

- [Larsen JB et al. Disseminated intravascular coagulation diagnosis: Positive predictive value of the ISTH score in a Danish population. Research and Practice in Thrombosis and Haemostasis, 2021. Table 1 (fibrinogen boundary).](https://doi.org/10.1002/rth2.12636)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
