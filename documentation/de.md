<!-- ELUCENIA technical documentation · apache-ii · de · no clinical/professional/rights approval -->

# APACHE II

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/apache-ii)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Alter

`idade`

Jahre · Bereich: 16–110

### Körperkerntemperatur

`temp`

°C · Bereich: 25–45

### Mittlerer arterieller Druck

`pam`

mmHg · Bereich: 20–250

### Herzfrequenz

`fc`

bpm · Bereich: 20–250

### Atemfrequenz

`fr`

Atemzüge/min · Bereich: 0–80

### FiO₂

`fio2`

% · Bereich: 21–100

### PaO₂

`pao2`

mmHg · Bereich: 20–700

### PaCO₂ (erforderlich bei FiO₂ ≥ 50 %)

`paco2`

mmHg · optional · Bereich: 10–150

### Arterieller pH-Wert

`ph`

Bereich: 6,5–8

### Natrium

`na`

mEq/L · Bereich: 90–200

### Kalium

`k`

mEq/L · Bereich: 1–10

### Kreatinin

`cr`

mg/dL · Bereich: 0,1–20

### Akutes Nierenversagen?

`ira`

- `0` — Nein
- `1` — Ja

### Hämatokrit

`ht`

% · Bereich: 5–75

### Leukozyten

`leuco`

×10³/µL · Bereich: 0,1–200

### Glasgow Coma Scale

`gcs`

Bereich: 3–15

### Vorbestehendes schweres Organversagen oder Immunsuppression (Zirrhose, NYHA IV, schwere COPD, chronische Dialyse, Immunsuppression)

`cronica`

- `0` — Nein
- `1` — Ja

### Aufnahmeart

`admissao`

- `clin` — Internistisch (nicht chirurgisch)
- `urg` — Nach Notfalloperation
- `elet` — Nach elektiver Operation

### Hauptdiagnosekategorie

`diag`

- `n_asma` — Internistisch · Ateminsuffizienz: Asthma oder Allergie
- `n_dpoc` — Internistisch · Ateminsuffizienz: COPD
- `n_edema` — Internistisch · Ateminsuffizienz: nichtkardiogenes Lungenödem
- `n_pcr_resp` — Internistisch · Ateminsuffizienz: nach Atemstillstand
- `n_aspiracao` — Internistisch · Ateminsuffizienz: Aspiration, Vergiftung oder toxische Exposition
- `n_tep` — Internistisch · Ateminsuffizienz: Lungenembolie
- `n_infec_resp` — Internistisch · Ateminsuffizienz: Infektion
- `n_neo_resp` — Internistisch · Ateminsuffizienz: Neoplasie
- `n_has` — Internistisch · Kardiovaskulär: Hypertonie
- `n_ritmo` — Internistisch · Kardiovaskulär: Herzrhythmusstörung
- `n_icc` — Internistisch · Kardiovaskulär: kongestive Herzinsuffizienz
- `n_hipovol` — Internistisch · Kardiovaskulär: hämorrhagischer Schock oder Hypovolämie
- `n_dac` — Internistisch · Kardiovaskulär: koronare Herzkrankheit
- `n_sepse` — Sepsis (internistisch oder postoperativ)
- `n_pcr` — Nach Herzstillstand (internistisch oder postoperativ)
- `n_cardiog` — Internistisch · Kardiovaskulär: kardiogener Schock
- `n_aneur` — Internistisch · Kardiovaskulär: Aortendissektion oder Aortenaneurysma
- `n_politrauma` — Internistisch · Trauma: Polytrauma
- `n_tce` — Internistisch · Trauma: Schädel-Hirn-Trauma
- `n_convulsao` — Internistisch · Neurologisch: Krampfanfall
- `n_hic` — Internistisch · Neurologisch: intrakranielle Blutung, Subarachnoidalblutung oder Subduralhämatom
- `n_intox` — Internistisch · Medikamenten- oder Drogenüberdosierung
- `n_cad` — Internistisch · Diabetische Ketoazidose
- `n_hda` — Internistisch · Gastrointestinale Blutung
- `n_outro_metab` — Internistisch · Sonstiges: metabolisch oder renal
- `n_outro_resp` — Internistisch · Sonstiges: respiratorisch
- `n_outro_neuro` — Internistisch · Sonstiges: neurologisch
- `n_outro_cv` — Internistisch · Sonstiges: kardiovaskulär
- `n_outro_gi` — Internistisch · Sonstiges: gastrointestinal
- `p_politrauma` — Postoperativ · Polytrauma
- `p_cv_cronica` — Postoperativ · Chronische Herz-Kreislauf-Erkrankung
- `p_vascular` — Postoperativ · Periphere Gefäßchirurgie
- `p_valva` — Postoperativ · Herzklappenoperation
- `p_cranio_neo` — Postoperativ · Kraniotomie bei Neoplasie
- `p_renal_neo` — Postoperativ · Nierenoperation bei Neoplasie
- `p_tx_renal` — Postoperativ · Nierentransplantation
- `p_tce` — Postoperativ · Schädel-Hirn-Trauma
- `p_torax_neo` — Postoperativ · Thoraxoperation bei Neoplasie
- `p_cranio_hic` — Postoperativ · Kraniotomie bei intrakranieller, Subarachnoidal- oder Subduralblutung
- `p_coluna` — Postoperativ · Laminektomie oder Rückenmarksoperation
- `p_choque` — Postoperativ · Hämorrhagischer Schock
- `p_hda` — Postoperativ · Gastrointestinale Blutung
- `p_gi_neo` — Postoperativ · Gastrointestinale Operation bei Neoplasie
- `p_insuf_resp` — Postoperativ · Ateminsuffizienz nach Operation
- `p_perfuracao` — Postoperativ · Gastrointestinale Perforation oder Obstruktion
- `p_outro_neuro` — Postoperativ · Sonstiges: neurologisch
- `p_outro_cv` — Postoperativ · Sonstiges: kardiovaskulär
- `p_outro_resp` — Postoperativ · Sonstiges: respiratorisch
- `p_outro_gi` — Postoperativ · Sonstiges: gastrointestinal
- `p_outro_metab` — Postoperativ · Sonstiges: metabolisch oder renal

## Fassung der Methode

APACHE II/Knaus 1985: 12 Variablen; Alter; chronische Erkrankung; Oxygenierung nach FiO₂; diagnoseabhängiges logistisches Modell

## Dokumentierte Formel

APACHE II = Akutphysiologiescore (12 Variablen, jeweils 0 bis 4 Punkte; Glasgow zählt als 15 − Glasgow) + Alterspunkte (≤ 44 = 0; 45–54 = 2; 55–64 = 3; 65–74 = 5; ≥ 75 = 6) + chronische Erkrankung (5 Punkte bei internistischer Aufnahme oder nach Notfalloperation; 2 nach elektiver Operation).

Oxygenierung: bei FiO₂ ≥ 50% den A–a-Gradienten bewerten \[FiO₂ × 713 − PaCO₂/0,8 − PaO₂\]: ≥ 500 = 4; 350–499 = 3; 200–349 = 2; \< 200 = 0. Bei FiO₂ \< 50% PaO₂ bewerten: \> 70 = 0; 61–70 = 1; 55–60 = 3; \< 55 = 4. Kreatininpunkte werden bei akutem Nierenversagen verdoppelt.

Vorhergesagte Krankenhaussterblichkeit: ln\[R/(1 − R)\] = −3,517 + 0,146 × APACHE II + 0,603 (bei Notfalloperation) + Gewicht der Diagnosekategorie.

## Grenzen und Population

APACHE II von 1985 wurde bei 5815 Intensivaufnahmen in 13 Krankenhäusern mit der Krankenhaussterblichkeit in Beziehung gesetzt. Die von den Autoren beschriebene prognostische Einteilung verbindet den Score mit einer genauen Krankheitsbeschreibung; die Summe allein bildet diese diagnostische Information nicht ab. Erfassungszeitraum, Ausschlüsse und Anwendbarkeit außerhalb dieser Population müssen im vollständigen Methodentext geprüft werden.

## Referenzen

- [Knaus WA, Draper EA, Wagner DP, Zimmerman JE. APACHE II: a severity of disease classification system. Crit Care Med, 1985.](https://doi.org/10.1097/00003246-198510000-00009)

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

Vorhergesagte Krankenhaussterblichkeit von 0,8%

| Ergebnisdetails | |
| --- | --- |
| Akutphysiologischer Score (APS) | 0 Punkte |
| Alter | 0 Punkte |
| Chronische Erkrankung | 0 Punkte |
| Vorhergesagte Krankenhaussterblichkeit | 0,8% |

Verwenden Sie die schlechtesten Werte der ersten 24 Stunden auf der Intensivstation. Die Vorhersage gilt für Patientengruppen, nicht für Entscheidungen im Einzelfall.


### 2

Vorhergesagte Krankenhaussterblichkeit von 25,6%

| Ergebnisdetails | |
| --- | --- |
| Akutphysiologischer Score (APS) | 13 Punkte |
| Alter | 3 Punkte |
| Chronische Erkrankung | 0 Punkte |
| Vorhergesagte Krankenhaussterblichkeit | 25,6% |

Verwenden Sie die schlechtesten Werte der ersten 24 Stunden auf der Intensivstation. Die Vorhersage gilt für Patientengruppen, nicht für Entscheidungen im Einzelfall.


### 3

Vorhergesagte Krankenhaussterblichkeit von 97,9%

| Ergebnisdetails | |
| --- | --- |
| Akutphysiologischer Score (APS) | 35 Punkte |
| A-a-Gradient (FiO₂ ≥ 50%) | 450 mmHg |
| Alter | 6 Punkte |
| Chronische Erkrankung | 5 Punkte |
| Vorhergesagte Krankenhaussterblichkeit | 97,9% |

Verwenden Sie die schlechtesten Werte der ersten 24 Stunden auf der Intensivstation. Die Vorhersage gilt für Patientengruppen, nicht für Entscheidungen im Einzelfall.

