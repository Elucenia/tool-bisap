<!-- ELUCENIA technical documentation · bisap · zh · no clinical/professional/rights approval -->

# BISAP 评分

[条件、来源与许可](https://elucenia.org/zh/tools/bisap)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 尿素 \> 53 mg/dL（BUN \> 25 mg/dL）

`bun`

### 精神状态改变（Glasgow \< 15）

`mental`

### SIRS（2 项或更多标准）

`sirs`

### 年龄 \> 60 岁

`idade`

### 影像显示胸腔积液

`derrame`

## 方法版本

BISAP/Wu 2008：5因素、最初24 h；BUN \>25 mg/dL；年龄\>60

## 已记录的公式

最初24小时各项1分：BUN \>25 mg/dL（尿素\>53 mg/dL）、I精神状态受损、SIRS、A年龄\>60岁、P胸腔积液。

SIRS：以下≥2项，体温\<36或\>38 °C、心率\>90 bpm、呼吸频率\>20次/分或PaCO₂ \<32 mmHg、白细胞\<4000或\>12000/mm³或杆状核细胞\>10%。

## 限制与适用人群

2008年的BISAP利用急性胰腺炎最初24小时的数据对院内死亡风险分层。血尿素氮（BUN）\>25 mg/dL和年龄\>60岁是评分项目，而非最低纳入条件。坏死、器官衰竭评估和亚组适用性应依据各自来源；观察到的发生率并不能确定个体预后。

## 参考文献

- [Wu BU et al. The early prediction of mortality in acute pancreatitis: a large population-based study. Gut, 2008.](https://doi.org/10.1136/gut.2008.152702)

- [Singh VK et al. A prospective evaluation of the bedside index for severity in acute pancreatitis score in assessing mortality and intermediate markers of severity in acute pancreatitis. Am J Gastroenterol, 2009.](https://doi.org/10.1038/ajg.2009.28)

- [Banks PA et al. Classification of acute pancreatitis—2012: revision of the Atlanta classification and definitions by international consensus. Gut, 2013.](https://doi.org/10.1136/gutjnl-2012-302779)

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
