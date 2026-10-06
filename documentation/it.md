<!-- ELUCENIA technical documentation · apache-ii · it · no clinical/professional/rights approval -->

# APACHE II

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/apache-ii)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Età

`idade`

anni · intervallo: 16–110

### Temperatura centrale

`temp`

°C · intervallo: 25–45

### Pressione arteriosa media

`pam`

mmHg · intervallo: 20–250

### Frequenza cardiaca

`fc`

bpm · intervallo: 20–250

### Frequenza respiratoria

`fr`

atti/min · intervallo: 0–80

### FiO₂

`fio2`

% · intervallo: 21–100

### PaO₂

`pao2`

mmHg · intervallo: 20–700

### PaCO₂ (necessaria se FiO₂ ≥ 50%)

`paco2`

mmHg · facoltativo · intervallo: 10–150

### pH arterioso

`ph`

intervallo: 6,5–8

### Sodio

`na`

mEq/L · intervallo: 90–200

### Potassio

`k`

mEq/L · intervallo: 1–10

### Creatinina

`cr`

mg/dL · intervallo: 0,1–20

### Insufficienza renale acuta?

`ira`

- `0` — No
- `1` — Sì

### Ematocrito

`ht`

% · intervallo: 5–75

### Leucociti

`leuco`

×10³/µL · intervallo: 0,1–200

### Scala del coma di Glasgow

`gcs`

intervallo: 3–15

### Insufficienza d’organo grave preesistente o immunosoppressione (cirrosi, NYHA IV, BPCO grave, dialisi cronica, immunosoppressione)

`cronica`

- `0` — No
- `1` — Sì

### Tipo di ricovero

`admissao`

- `clin` — Medico (non chirurgico)
- `urg` — Dopo chirurgia d’urgenza
- `elet` — Postoperatorio elettivo

### Categoria diagnostica principale

`diag`

- `n_asma` — Medico · Insufficienza respiratoria: asma o allergia
- `n_dpoc` — Medico · Insufficienza respiratoria: BPCO
- `n_edema` — Medico · Insufficienza respiratoria: edema polmonare non cardiogeno
- `n_pcr_resp` — Medico · Insufficienza respiratoria: dopo arresto respiratorio
- `n_aspiracao` — Medico · Insufficienza respiratoria: aspirazione, intossicazione o esposizione tossica
- `n_tep` — Medico · Insufficienza respiratoria: embolia polmonare
- `n_infec_resp` — Medico · Insufficienza respiratoria: infezione
- `n_neo_resp` — Medico · Insufficienza respiratoria: neoplasia
- `n_has` — Medico · Cardiovascolare: ipertensione
- `n_ritmo` — Medico · Cardiovascolare: disturbo del ritmo
- `n_icc` — Medico · Cardiovascolare: insufficienza cardiaca congestizia
- `n_hipovol` — Medico · Cardiovascolare: shock emorragico o ipovolemia
- `n_dac` — Medico · Cardiovascolare: coronaropatia
- `n_sepse` — Sepsi (paziente medico o postoperatorio)
- `n_pcr` — Dopo arresto cardiaco (paziente medico o postoperatorio)
- `n_cardiog` — Medico · Cardiovascolare: shock cardiogeno
- `n_aneur` — Medico · Cardiovascolare: dissezione o aneurisma aortico
- `n_politrauma` — Medico · Trauma: politrauma
- `n_tce` — Medico · Trauma: trauma cranioencefalico
- `n_convulsao` — Medico · Neurologico: crisi convulsiva
- `n_hic` — Medico · Neurologico: emorragia intracranica, emorragia subaracnoidea o ematoma subdurale
- `n_intox` — Medico · Sovradosaggio di farmaci o droghe
- `n_cad` — Medico · Chetoacidosi diabetica
- `n_hda` — Medico · Emorragia gastrointestinale
- `n_outro_metab` — Medico · Altro: metabolico o renale
- `n_outro_resp` — Medico · Altro: respiratorio
- `n_outro_neuro` — Medico · Altro: neurologico
- `n_outro_cv` — Medico · Altro: cardiovascolare
- `n_outro_gi` — Medico · Altro: gastrointestinale
- `p_politrauma` — Postoperatorio · Politrauma
- `p_cv_cronica` — Postoperatorio · Malattia cardiovascolare cronica
- `p_vascular` — Postoperatorio · Chirurgia vascolare periferica
- `p_valva` — Postoperatorio · Chirurgia valvolare cardiaca
- `p_cranio_neo` — Postoperatorio · Craniotomia per neoplasia
- `p_renal_neo` — Postoperatorio · Chirurgia renale per neoplasia
- `p_tx_renal` — Postoperatorio · Trapianto renale
- `p_tce` — Postoperatorio · Trauma cranioencefalico
- `p_torax_neo` — Postoperatorio · Chirurgia toracica per neoplasia
- `p_cranio_hic` — Postoperatorio · Craniotomia per emorragia intracranica, subaracnoidea o subdurale
- `p_coluna` — Postoperatorio · Laminectomia o chirurgia del midollo spinale
- `p_choque` — Postoperatorio · Shock emorragico
- `p_hda` — Postoperatorio · Emorragia digestiva
- `p_gi_neo` — Postoperatorio · Chirurgia gastrointestinale per neoplasia
- `p_insuf_resp` — Postoperatorio · Insufficienza respiratoria dopo chirurgia
- `p_perfuracao` — Postoperatorio · Perforazione od ostruzione gastrointestinale
- `p_outro_neuro` — Postoperatorio · Altro: neurologico
- `p_outro_cv` — Postoperatorio · Altro: cardiovascolare
- `p_outro_resp` — Postoperatorio · Altro: respiratorio
- `p_outro_gi` — Postoperatorio · Altro: gastrointestinale
- `p_outro_metab` — Postoperatorio · Altro: metabolico o renale

## Edizione del metodo

APACHE II/Knaus 1985: 12 variabili; età; malattia cronica; ossigenazione secondo FiO₂; modello logistico diagnostico

## Formula documentata

APACHE II = punteggio fisiologico acuto (12 variabili, ciascuna da 0 a 4 punti; Glasgow contribuisce come 15 − Glasgow) + punti per età (≤ 44 = 0; 45–54 = 2; 55–64 = 3; 65–74 = 5; ≥ 75 = 6) + malattia cronica (5 punti nel ricovero medico o dopo chirurgia d’urgenza; 2 dopo chirurgia elettiva).

Ossigenazione: con FiO₂ ≥ 50%, assegnare punti al gradiente A–a \[FiO₂ × 713 − PaCO₂/0,8 − PaO₂\]: ≥ 500 = 4; 350–499 = 3; 200–349 = 2; \< 200 = 0. Con FiO₂ \< 50%, assegnare punti alla PaO₂: \> 70 = 0; 61–70 = 1; 55–60 = 3; \< 55 = 4. I punti della creatinina raddoppiano nell’insufficienza renale acuta.

Mortalità ospedaliera prevista: ln\[R/(1 − R)\] = −3,517 + 0,146 × APACHE II + 0,603 (se chirurgia d’urgenza) + peso della categoria diagnostica.

## Limiti e popolazione

L’APACHE II del 1985 è stato associato alla mortalità ospedaliera in 5815 ricoveri in terapia intensiva di 13 ospedali. La stratificazione prognostica descritta dagli autori combina il punteggio con una descrizione precisa della malattia; il totale da solo non riproduce tale informazione diagnostica. La finestra di raccolta, le esclusioni e l’applicabilità al di fuori di questa popolazione richiedono una verifica nel metodo completo.

## Riferimenti

- [Knaus WA, Draper EA, Wagner DP, Zimmerman JE. APACHE II: a severity of disease classification system. Crit Care Med, 1985.](https://doi.org/10.1097/00003246-198510000-00009)

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

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Mortalità ospedaliera prevista del 0,8%

| Dettagli del risultato | |
| --- | --- |
| Punteggio di fisiologia acuta (APS) | 0 punti |
| Età | 0 punti |
| Malattia cronica | 0 punti |
| Mortalità ospedaliera prevista | 0,8% |

Usare i valori peggiori delle prime 24 ore in terapia intensiva. La previsione vale per gruppi di pazienti, non per decidere condotte individuali.


### 2

Mortalità ospedaliera prevista del 25,6%

| Dettagli del risultato | |
| --- | --- |
| Punteggio di fisiologia acuta (APS) | 13 punti |
| Età | 3 punti |
| Malattia cronica | 0 punti |
| Mortalità ospedaliera prevista | 25,6% |

Usare i valori peggiori delle prime 24 ore in terapia intensiva. La previsione vale per gruppi di pazienti, non per decidere condotte individuali.


### 3

Mortalità ospedaliera prevista del 97,9%

| Dettagli del risultato | |
| --- | --- |
| Punteggio di fisiologia acuta (APS) | 35 punti |
| Gradiente A-a (FiO₂ ≥ 50%) | 450 mmHg |
| Età | 6 punti |
| Malattia cronica | 5 punti |
| Mortalità ospedaliera prevista | 97,9% |

Usare i valori peggiori delle prime 24 ore in terapia intensiva. La previsione vale per gruppi di pazienti, non per decidere condotte individuali.

