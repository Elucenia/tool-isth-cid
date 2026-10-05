<!-- ELUCENIA technical documentation · isth-cid · fr · no clinical/professional/rights approval -->

# Score ISTH de CIVD manifeste

[conditions, sources et autorisations](https://elucenia.org/fr/outils/isth-cid)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Plaquettes

`plaq`

- `0` — \> 100 000/µL
- `1` — 50 000 à 100 000/µL
- `2` — \< 50 000/µL

### Marqueur de fibrine (D-dimères ou produits de dégradation de la fibrine)

`dd`

- `0` — Pas d’augmentation
- `2` — Augmentation modérée
- `3` — Augmentation marquée

### Allongement du temps de prothrombine

`tp`

- `0` — \< 3 s
- `1` — 3 à 6 s
- `2` — \> 6 s

### Fibrinogène

`fib`

- `0` — ≥ 1 g/L
- `1` — \< 1 g/L (100 mg/dL)

## Édition de la méthode

ISTH/Taylor 2001 : CIVD manifeste, plaquettes/PDF/temps de prothrombine/fibrinogène, total 0–8

## Formule documentée

Plaquettes \> 100 mille 0, 50–100 mille 1, \< 50 mille 2 · D-dimère/PDF sans hausse 0, modérée 2, marquée 3 · allongement du temps de prothrombine \< 3 s 0, 3–6 s 1, \> 6 s 2 · fibrinogène ≥ 1 g/L 0, \< 1 g/L 1. Maximum : 8.

Prérequis : maladie sous-jacente associée à CIVD (sepsis, traumatisme, cancer, complication obstétricale, etc.).

## Limites et population

Appliquer dans le contexte d’une maladie sous-jacente compatible avec une CIVD, en combinant données cliniques et biologiques. Le processus est dynamique et exige des évaluations répétées. Un score ne démontre pas seul le diagnostic ; la précision varie selon la population et la strate de score.

## Références

- [Taylor FB Jr et al. Towards definition, clinical and laboratory criteria, and a scoring system for disseminated intravascular coagulation. Thromb Haemost, 2001.](https://doi.org/10.1055/s-0037-1616068)

- [Levi M et al. Guidelines for the diagnosis and management of disseminated intravascular coagulation. Br J Haematol, 2009.](https://doi.org/10.1111/j.1365-2141.2009.07600.x)

- [Larsen JB et al. Disseminated intravascular coagulation diagnosis: Positive predictive value of the ISTH score in a Danish population. Research and Practice in Thrombosis and Haemostasis, 2021. Table 1 (fibrinogen boundary).](https://doi.org/10.1002/rth2.12636)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
