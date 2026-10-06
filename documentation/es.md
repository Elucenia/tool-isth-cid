<!-- ELUCENIA technical documentation · isth-cid · es · no clinical/professional/rights approval -->

# Puntuación ISTH de CID manifiesta

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/isth-cid)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Plaquetas

`plaq`

- `0` — \> 100.000/µL
- `1` — 50.000 a 100.000/µL
- `2` — \< 50.000/µL

### Marcador de fibrina (dímero D o productos de degradación de fibrina)

`dd`

- `0` — Sin aumento
- `2` — Aumento moderado
- `3` — Aumento marcado

### Prolongación del tiempo de protrombina

`tp`

- `0` — \< 3 s
- `1` — 3 a 6 s
- `2` — \> 6 s

### Fibrinógeno

`fib`

- `0` — ≥ 1 g/L
- `1` — \< 1 g/L (100 mg/dL)

## Edición del método

ISTH/Taylor 2001: CID manifiesta, plaquetas/PDF/TP/fibrinógeno, total 0–8

## Fórmula documentada

Plaquetas \> 100 mil 0, 50–100 mil 1, \< 50 mil 2 · dímero D/PDF sin aumento 0, moderado 2, marcado 3 · prolongación TP \< 3 s 0, 3–6 s 1, \> 6 s 2 · fibrinógeno ≥ 1 g/L 0, \< 1 g/L 1. Máximo: 8.

Requisito: enfermedad de base asociada a CID (sepsis, traumatismo, cáncer, complicación obstétrica, etc.).

## Límites y población

Aplíquelo en el contexto de una enfermedad de base compatible con CID, combinando datos clínicos y de laboratorio. El proceso es dinámico y requiere repetir la evaluación. Una puntuación no demuestra por sí sola el diagnóstico; la precisión varía con la población y el estrato de puntuación.

## Referencias

- [Taylor FB Jr et al. Towards definition, clinical and laboratory criteria, and a scoring system for disseminated intravascular coagulation. Thromb Haemost, 2001.](https://doi.org/10.1055/s-0037-1616068)

- [Levi M et al. Guidelines for the diagnosis and management of disseminated intravascular coagulation. Br J Haematol, 2009.](https://doi.org/10.1111/j.1365-2141.2009.07600.x)

- [Larsen JB et al. Disseminated intravascular coagulation diagnosis: Positive predictive value of the ISTH score in a Danish population. Research and Practice in Thrombosis and Haemostasis, 2021. Table 1 (fibrinogen boundary).](https://doi.org/10.1002/rth2.12636)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

No compatible con CID manifiesta (< 5)

Sugiere, pero no descarta, CID no manifiesta: repetir en 1 a 2 días.


### 2

Compatible con CID manifiesta (≥ 5)

Tratar la causa de base; repetir el puntaje diariamente.


### 3

Compatible con CID manifiesta (≥ 5)

Tratar la causa de base; repetir el puntaje diariamente.

