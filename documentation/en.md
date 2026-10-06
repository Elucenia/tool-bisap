<!-- ELUCENIA technical documentation · bisap · en · no clinical/professional/rights approval -->

# BISAP score

[conditions, sources and permissions](https://elucenia.org/en/tools/bisap)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Urea \> 53 mg/dL (BUN \> 25 mg/dL)

`bun`

### Altered mental status (Glasgow \< 15)

`mental`

### SIRS (2 or more criteria)

`sirs`

### Age \> 60 years

`idade`

### Pleural effusion on imaging

`derrame`

## Method edition

BISAP/Wu 2008: 5 factors, first 24 h; BUN \>25 mg/dL; age \>60

## Documented formula

1 point for each item within 24 hours: BUN \>25 mg/dL (urea \>53 mg/dL), Impaired mental status, SIRS, Age \>60 years, Pleural effusion.

SIRS: ≥2 of temperature \<36 or \>38 °C, HR \>90 bpm, RR \>20 breaths/min or PaCO₂ \<32 mmHg, leukocytes \<4,000 or \>12,000/mm³ or \>10% bands.

## Limits and population

The 2008 BISAP uses data from the first 24 hours of acute pancreatitis to stratify in-hospital mortality risk. BUN \>25 mg/dL and age \>60 years are score items, not minimum inclusion criteria. Assessment of necrosis, organ failure and applicability to subgroups depend on their respective sources; observed rates do not establish individual prognostic certainty.

## References

- [Wu BU et al. The early prediction of mortality in acute pancreatitis: a large population-based study. Gut, 2008.](https://doi.org/10.1136/gut.2008.152702)

- [Singh VK et al. A prospective evaluation of the bedside index for severity in acute pancreatitis score in assessing mortality and intermediate markers of severity in acute pancreatitis. Am J Gastroenterol, 2009.](https://doi.org/10.1038/ajg.2009.28)

- [Banks PA et al. Classification of acute pancreatitis—2012: revision of the Atlanta classification and definitions by international consensus. Gut, 2013.](https://doi.org/10.1136/gutjnl-2012-302779)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

BISAP 0 to 2: lower mortality risk

Mortality below 1% in the derivation low-risk group; maintain clinical reassessment in the first 48 h.


### 2

BISAP ≥ 3: increased risk of mortality and complications

Associated with organ failure (OR 7,4), persistent failure (OR 12,7) and pancreatic necrosis (OR 3,8); consider ICU or intermediate care unit.

