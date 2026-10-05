<!-- ELUCENIA technical documentation · isth-cid · it · no clinical/professional/rights approval -->

# Punteggio ISTH di CID manifesta

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/isth-cid)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Piastrine

`plaq`

- `0` — \> 100.000/µL
- `1` — 50.000 a 100.000/µL
- `2` — \< 50.000/µL

### Marcatore della fibrina (D-dimero o prodotti di degradazione della fibrina)

`dd`

- `0` — Nessun aumento
- `2` — Aumento moderato
- `3` — Aumento marcato

### Prolungamento del tempo di protrombina

`tp`

- `0` — \< 3 s
- `1` — 3 a 6 s
- `2` — \> 6 s

### Fibrinogeno

`fib`

- `0` — ≥ 1 g/L
- `1` — \< 1 g/L (100 mg/dL)

## Edizione del metodo

ISTH/Taylor 2001: CID manifesta, piastrine/PDF/TP/fibrinogeno, totale 0–8

## Formula documentata

Piastrine \> 100 mila 0, 50–100 mila 1, \< 50 mila 2 · D-dimero/PDF senza aumento 0, moderato 2, marcato 3 · prolungamento TP \< 3 s 0, 3–6 s 1, \> 6 s 2 · fibrinogeno ≥ 1 g/L 0, \< 1 g/L 1. Massimo: 8.

Prerequisito: malattia di base associata a CID (sepsi, trauma, cancro, complicanza ostetrica ecc.).

## Limiti e popolazione

Applicare nel contesto di una malattia di base compatibile con CID, combinando dati clinici e di laboratorio. Il processo è dinamico e richiede la ripetizione della valutazione. Un punteggio da solo non dimostra la diagnosi; l’accuratezza varia con la popolazione e la fascia di punteggio.

## Riferimenti

- [Taylor FB Jr et al. Towards definition, clinical and laboratory criteria, and a scoring system for disseminated intravascular coagulation. Thromb Haemost, 2001.](https://doi.org/10.1055/s-0037-1616068)

- [Levi M et al. Guidelines for the diagnosis and management of disseminated intravascular coagulation. Br J Haematol, 2009.](https://doi.org/10.1111/j.1365-2141.2009.07600.x)

- [Larsen JB et al. Disseminated intravascular coagulation diagnosis: Positive predictive value of the ISTH score in a Danish population. Research and Practice in Thrombosis and Haemostasis, 2021. Table 1 (fibrinogen boundary).](https://doi.org/10.1002/rth2.12636)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
