<!-- ELUCENIA technical documentation · isth-cid · de · no clinical/professional/rights approval -->

# ISTH-Score für manifeste DIC

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/isth-cid)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Thrombozyten

`plaq`

- `0` — \> 100.000/µL
- `1` — 50.000 bis 100.000/µL
- `2` — \< 50.000/µL

### Fibrinmarker (D-Dimer oder Fibrinspaltprodukte)

`dd`

- `0` — Keine Zunahme
- `2` — Mäßige Zunahme
- `3` — Ausgeprägte Zunahme

### Verlängerung der Prothrombinzeit

`tp`

- `0` — \< 3 s
- `1` — 3 bis 6 s
- `2` — \> 6 s

### Fibrinogen

`fib`

- `0` — ≥ 1 g/L
- `1` — \< 1 g/L (100 mg/dL)

## Fassung der Methode

ISTH/Taylor 2001: manifeste DIC, Thrombozyten/FDP/PT/Fibrinogen, Gesamt 0–8

## Dokumentierte Formel

Thrombozyten \> 100 Tausend 0, 50–100 Tausend 1, \< 50 Tausend 2 · D-Dimer/FDP ohne Anstieg 0, mäßig 2, stark 3 · Prothrombinzeit-Verlängerung \< 3 s 0, 3–6 s 1, \> 6 s 2 · Fibrinogen ≥ 1 g/L 0, \< 1 g/L 1. Maximum: 8.

Voraussetzung: DIC-assoziierte Grunderkrankung (Sepsis, Trauma, Krebs, geburtshilfliche Komplikation usw.).

## Grenzen und Population

Im Kontext einer mit DIC vereinbaren Grunderkrankung unter Kombination klinischer und Labordaten anwenden. Der Prozess ist dynamisch und erfordert wiederholte Beurteilung. Ein Score allein belegt die Diagnose nicht; die Genauigkeit variiert mit Population und Scorestratum.

## Referenzen

- [Taylor FB Jr et al. Towards definition, clinical and laboratory criteria, and a scoring system for disseminated intravascular coagulation. Thromb Haemost, 2001.](https://doi.org/10.1055/s-0037-1616068)

- [Levi M et al. Guidelines for the diagnosis and management of disseminated intravascular coagulation. Br J Haematol, 2009.](https://doi.org/10.1111/j.1365-2141.2009.07600.x)

- [Larsen JB et al. Disseminated intravascular coagulation diagnosis: Positive predictive value of the ISTH score in a Danish population. Research and Practice in Thrombosis and Haemostasis, 2021. Table 1 (fibrinogen boundary).](https://doi.org/10.1002/rth2.12636)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Nicht vereinbar mit manifester DIC (< 5)

Spricht für eine nicht manifeste DIC, schließt sie aber nicht aus: in 1 bis 2 Tagen wiederholen.


### 2

Vereinbar mit manifester DIC (≥ 5)

Die Grunderkrankung behandeln; den Score täglich wiederholen.


### 3

Vereinbar mit manifester DIC (≥ 5)

Die Grunderkrankung behandeln; den Score täglich wiederholen.

