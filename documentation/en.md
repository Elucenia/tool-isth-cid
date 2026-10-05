<!-- ELUCENIA technical documentation · isth-cid · en · no clinical/professional/rights approval -->

# ISTH overt DIC score

[conditions, sources and permissions](https://elucenia.org/en/tools/isth-cid)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Platelets

`plaq`

- `0` — \> 100,000/µL
- `1` — 50,000 to 100,000/µL
- `2` — \< 50,000/µL

### Fibrin marker (D-dimer or fibrin degradation products)

`dd`

- `0` — No increase
- `2` — Moderate increase
- `3` — Marked increase

### Prothrombin time prolongation

`tp`

- `0` — \< 3 s
- `1` — 3 to 6 s
- `2` — \> 6 s

### Fibrinogen

`fib`

- `0` — ≥ 1 g/L
- `1` — \< 1 g/L (100 mg/dL)

## Method edition

ISTH/Taylor 2001: overt DIC, platelets/FDP/PT/fibrinogen, total 0–8

## Documented formula

Platelets \> 100 thousand 0, 50–100 thousand 1, \< 50 thousand 2 · D-dimer/FDP no rise 0, moderate 2, marked 3 · PT prolongation \< 3 s 0, 3–6 s 1, \> 6 s 2 · fibrinogen ≥ 1 g/L 0, \< 1 g/L 1. Maximum: 8.

Prerequisite: DIC-associated underlying disease (sepsis, trauma, cancer, obstetric complication, etc.).

## Limits and population

Apply in the context of an underlying disease compatible with DIC, combining clinical and laboratory data. The process is dynamic and requires repeated assessment. A score alone does not establish the diagnosis; accuracy varies with population and score stratum.

## References

- [Taylor FB Jr et al. Towards definition, clinical and laboratory criteria, and a scoring system for disseminated intravascular coagulation. Thromb Haemost, 2001.](https://doi.org/10.1055/s-0037-1616068)

- [Levi M et al. Guidelines for the diagnosis and management of disseminated intravascular coagulation. Br J Haematol, 2009.](https://doi.org/10.1111/j.1365-2141.2009.07600.x)

- [Larsen JB et al. Disseminated intravascular coagulation diagnosis: Positive predictive value of the ISTH score in a Danish population. Research and Practice in Thrombosis and Haemostasis, 2021. Table 1 (fibrinogen boundary).](https://doi.org/10.1002/rth2.12636)

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
