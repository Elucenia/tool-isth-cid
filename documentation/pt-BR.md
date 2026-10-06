<!-- ELUCENIA technical documentation · isth-cid · pt-BR · no clinical/professional/rights approval -->

# Escore ISTH de CID manifesta

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/isth-cid)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Plaquetas

`plaq`

- `0` — \> 100.000/µL
- `1` — 50.000 a 100.000/µL
- `2` — \< 50.000/µL

### Marcador de fibrina (D-dímero ou PDF)

`dd`

- `0` — Sem aumento
- `2` — Aumento moderado
- `3` — Aumento acentuado

### Prolongamento do tempo de protrombina

`tp`

- `0` — \< 3 s
- `1` — 3 a 6 s
- `2` — \> 6 s

### Fibrinogênio

`fib`

- `0` — ≥ 1 g/L
- `1` — \< 1 g/L (100 mg/dL)

## Edição do método

ISTH/Taylor 2001:CIDmanifesta, plaquetas/PDF/TP/fibrinogênio, total 0–8

## Fórmula documentada

Plaquetas \> 100 mil 0, 50–100 mil 1, \< 50 mil 2 · D-dímero/PDF sem aumento 0, moderado 2, acentuado 3 · TP prolongado \< 3 s 0, 3–6 s 1, \> 6 s 2 · fibrinogênio ≥ 1 g/L 0, \< 1 g/L 1. Máximo: 8.

Pré-requisito: doença de base associada a CID (sepse, trauma, câncer, complicação obstétrica etc.).

## Limites e população

Aplicar no contexto de doença de base compatível com CID, combinando dados clínicos e laboratoriais. O processo é dinâmico e requer repetição da avaliação. Um escore não comprova sozinho o diagnóstico; a precisão varia com a população e o estrato de pontuação.

## Referências

- [Taylor FB Jr et al. Towards definition, clinical and laboratory criteria, and a scoring system for disseminated intravascular coagulation. Thromb Haemost, 2001.](https://doi.org/10.1055/s-0037-1616068)

- [Levi M et al. Guidelines for the diagnosis and management of disseminated intravascular coagulation. Br J Haematol, 2009.](https://doi.org/10.1111/j.1365-2141.2009.07600.x)

- [Larsen JB et al. Disseminated intravascular coagulation diagnosis: Positive predictive value of the ISTH score in a Danish population. Research and Practice in Thrombosis and Haemostasis, 2021. Table 1 (fibrinogen boundary).](https://doi.org/10.1002/rth2.12636)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Não compatível com CID manifesta (< 5)

Sugere, mas não afasta, CID não manifesta: repetir em 1 a 2 dias.


### 2

Compatível com CID manifesta (≥ 5)

Tratar a causa de base; repetir o escore diariamente.


### 3

Compatível com CID manifesta (≥ 5)

Tratar a causa de base; repetir o escore diariamente.

