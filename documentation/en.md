<!-- ELUCENIA technical documentation · apache-ii · en · no clinical/professional/rights approval -->

# APACHE II

[conditions, sources and permissions](https://elucenia.org/en/tools/apache-ii)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Age

`idade`

years · range: 16–110

### Core temperature

`temp`

°C · range: 25–45

### Mean arterial pressure

`pam`

mmHg · range: 20–250

### Heart rate

`fc`

bpm · range: 20–250

### Respiratory rate

`fr`

breaths/min · range: 0–80

### FiO₂

`fio2`

% · range: 21–100

### PaO₂

`pao2`

mmHg · range: 20–700

### PaCO₂ (required if FiO₂ ≥ 50%)

`paco2`

mmHg · optional · range: 10–150

### Arterial pH

`ph`

range: 6.5–8

### Sodium

`na`

mEq/L · range: 90–200

### Potassium

`k`

mEq/L · range: 1–10

### Creatinine

`cr`

mg/dL · range: 0.1–20

### Acute kidney injury?

`ira`

- `0` — No
- `1` — Yes

### Hematocrit

`ht`

% · range: 5–75

### White blood cells

`leuco`

×10³/µL · range: 0.1–200

### Glasgow Coma Scale

`gcs`

range: 3–15

### Pre-existing severe organ failure or immunosuppression (cirrhosis, NYHA IV, severe COPD, chronic dialysis, immunosuppression)

`cronica`

- `0` — No
- `1` — Yes

### Admission type

`admissao`

- `clin` — Medical (non-surgical)
- `urg` — After emergency surgery
- `elet` — After elective surgery

### Principal diagnostic category

`diag`

- `n_asma` — Medical · Respiratory failure: asthma or allergy
- `n_dpoc` — Medical · Respiratory failure: COPD
- `n_edema` — Medical · Respiratory failure: noncardiogenic pulmonary edema
- `n_pcr_resp` — Medical · Respiratory failure: after respiratory arrest
- `n_aspiracao` — Medical · Respiratory failure: aspiration, poisoning or toxic exposure
- `n_tep` — Medical · Respiratory failure: pulmonary embolism
- `n_infec_resp` — Medical · Respiratory failure: infection
- `n_neo_resp` — Medical · Respiratory failure: neoplasm
- `n_has` — Medical · Cardiovascular: hypertension
- `n_ritmo` — Medical · Cardiovascular: rhythm disorder
- `n_icc` — Medical · Cardiovascular: congestive heart failure
- `n_hipovol` — Medical · Cardiovascular: hemorrhagic shock or hypovolemia
- `n_dac` — Medical · Cardiovascular: coronary artery disease
- `n_sepse` — Sepsis (medical or postoperative)
- `n_pcr` — After cardiac arrest (medical or postoperative)
- `n_cardiog` — Medical · Cardiovascular: cardiogenic shock
- `n_aneur` — Medical · Cardiovascular: aortic dissection or aneurysm
- `n_politrauma` — Medical · Trauma: multiple trauma
- `n_tce` — Medical · Trauma: traumatic brain injury
- `n_convulsao` — Medical · Neurological: seizure
- `n_hic` — Medical · Neurological: intracranial hemorrhage, subarachnoid hemorrhage or subdural hematoma
- `n_intox` — Medical · Drug overdose
- `n_cad` — Medical · Diabetic ketoacidosis
- `n_hda` — Medical · Gastrointestinal bleeding
- `n_outro_metab` — Medical · Other: metabolic or renal
- `n_outro_resp` — Medical · Other: respiratory
- `n_outro_neuro` — Medical · Other: neurological
- `n_outro_cv` — Medical · Other: cardiovascular
- `n_outro_gi` — Medical · Other: gastrointestinal
- `p_politrauma` — Postoperative · Multiple trauma
- `p_cv_cronica` — Postoperative · Chronic cardiovascular disease
- `p_vascular` — Postoperative · Peripheral vascular surgery
- `p_valva` — Postoperative · Heart valve surgery
- `p_cranio_neo` — Postoperative · Craniotomy for neoplasm
- `p_renal_neo` — Postoperative · Renal surgery for neoplasm
- `p_tx_renal` — Postoperative · Kidney transplantation
- `p_tce` — Postoperative · Traumatic brain injury
- `p_torax_neo` — Postoperative · Thoracic surgery for neoplasm
- `p_cranio_hic` — Postoperative · Craniotomy for intracranial, subarachnoid or subdural hemorrhage
- `p_coluna` — Postoperative · Laminectomy or spinal cord surgery
- `p_choque` — Postoperative · Hemorrhagic shock
- `p_hda` — Postoperative · Gastrointestinal bleeding
- `p_gi_neo` — Postoperative · Gastrointestinal surgery for neoplasm
- `p_insuf_resp` — Postoperative · Respiratory failure after surgery
- `p_perfuracao` — Postoperative · Gastrointestinal perforation or obstruction
- `p_outro_neuro` — Postoperative · Other: neurological
- `p_outro_cv` — Postoperative · Other: cardiovascular
- `p_outro_resp` — Postoperative · Other: respiratory
- `p_outro_gi` — Postoperative · Other: gastrointestinal
- `p_outro_metab` — Postoperative · Other: metabolic or renal

## Method edition

APACHE II/Knaus 1985: 12 variables; age; chronic disease; oxygenation by FiO₂; diagnosis-specific logistic model

## Documented formula

APACHE II = acute physiology score (12 variables, 0 to 4 points each; Glasgow contributes 15 − Glasgow) + age points (≤ 44 = 0; 45–54 = 2; 55–64 = 3; 65–74 = 5; ≥ 75 = 6) + chronic disease (5 points for medical admission or after emergency surgery; 2 points after elective surgery).

Oxygenation: with FiO₂ ≥ 50%, score the A–a gradient \[FiO₂ × 713 − PaCO₂/0.8 − PaO₂\]: ≥ 500 = 4; 350–499 = 3; 200–349 = 2; \< 200 = 0. With FiO₂ \< 50%, score PaO₂: \> 70 = 0; 61–70 = 1; 55–60 = 3; \< 55 = 4. Creatinine points are doubled in acute renal failure.

Predicted hospital mortality: ln\[R/(1 − R)\] = −3.517 + 0.146 × APACHE II + 0.603 (if emergency surgery) + diagnostic-category weight.

## Limits and population

APACHE II from 1985 was associated with hospital mortality in 5815 ICU admissions at 13 hospitals. The prognostic stratification described by the authors combines the score with a precise description of the disease; the total alone does not reproduce that diagnostic information. The collection window, exclusions and applicability outside this population require checking in the full method.

## References

- [Knaus WA, Draper EA, Wagner DP, Zimmerman JE. APACHE II: a severity of disease classification system. Crit Care Med, 1985.](https://doi.org/10.1097/00003246-198510000-00009)

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
