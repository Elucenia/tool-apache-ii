<!-- ELUCENIA technical documentation · apache-ii · es · no clinical/professional/rights approval -->

# APACHE II

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/apache-ii)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Edad

`idade`

años · intervalo: 16–110

### Temperatura central

`temp`

°C · intervalo: 25–45

### Presión arterial media

`pam`

mmHg · intervalo: 20–250

### Frecuencia cardíaca

`fc`

bpm · intervalo: 20–250

### Frecuencia respiratoria

`fr`

respiraciones/min · intervalo: 0–80

### FiO₂

`fio2`

% · intervalo: 21–100

### PaO₂

`pao2`

mmHg · intervalo: 20–700

### PaCO₂ (necesaria si FiO₂ ≥ 50%)

`paco2`

mmHg · opcional · intervalo: 10–150

### pH arterial

`ph`

intervalo: 6,5–8

### Sodio

`na`

mEq/L · intervalo: 90–200

### Potasio

`k`

mEq/L · intervalo: 1–10

### Creatinina

`cr`

mg/dL · intervalo: 0,1–20

### ¿Lesión renal aguda?

`ira`

- `0` — No
- `1` — Sí

### Hematocrito

`ht`

% · intervalo: 5–75

### Leucocitos

`leuco`

×10³/µL · intervalo: 0,1–200

### Escala de coma de Glasgow

`gcs`

intervalo: 3–15

### Insuficiencia orgánica grave previa o inmunosupresión (cirrosis, NYHA IV, EPOC grave, diálisis crónica, inmunosupresión)

`cronica`

- `0` — No
- `1` — Sí

### Tipo de ingreso

`admissao`

- `clin` — Médico (no quirúrgico)
- `urg` — Tras cirugía de urgencia
- `elet` — Posoperatorio electivo

### Categoría diagnóstica principal

`diag`

- `n_asma` — Médico · Insuficiencia respiratoria: asma o alergia
- `n_dpoc` — Médico · Insuficiencia respiratoria: EPOC
- `n_edema` — Médico · Insuficiencia respiratoria: edema pulmonar no cardiogénico
- `n_pcr_resp` — Médico · Insuficiencia respiratoria: tras parada respiratoria
- `n_aspiracao` — Médico · Insuficiencia respiratoria: aspiración, intoxicación o exposición a tóxicos
- `n_tep` — Médico · Insuficiencia respiratoria: embolia pulmonar
- `n_infec_resp` — Médico · Insuficiencia respiratoria: infección
- `n_neo_resp` — Médico · Insuficiencia respiratoria: neoplasia
- `n_has` — Médico · Cardiovascular: hipertensión
- `n_ritmo` — Médico · Cardiovascular: trastorno del ritmo
- `n_icc` — Médico · Cardiovascular: insuficiencia cardíaca congestiva
- `n_hipovol` — Médico · Cardiovascular: shock hemorrágico o hipovolemia
- `n_dac` — Médico · Cardiovascular: enfermedad coronaria
- `n_sepse` — Sepsis (paciente médico o posoperatorio)
- `n_pcr` — Tras parada cardíaca (paciente médico o posoperatorio)
- `n_cardiog` — Médico · Cardiovascular: shock cardiogénico
- `n_aneur` — Médico · Cardiovascular: disección o aneurisma aórtico
- `n_politrauma` — Médico · Trauma: politraumatismo
- `n_tce` — Médico · Trauma: traumatismo craneoencefálico
- `n_convulsao` — Médico · Neurológico: crisis convulsiva
- `n_hic` — Médico · Neurológico: hemorragia intracraneal, hemorragia subaracnoidea o hematoma subdural
- `n_intox` — Médico · Sobredosis de fármacos o drogas
- `n_cad` — Médico · Cetoacidosis diabética
- `n_hda` — Médico · Hemorragia digestiva
- `n_outro_metab` — Médico · Otro: metabólico o renal
- `n_outro_resp` — Médico · Otro: respiratorio
- `n_outro_neuro` — Médico · Otro: neurológico
- `n_outro_cv` — Médico · Otro: cardiovascular
- `n_outro_gi` — Médico · Otro: gastrointestinal
- `p_politrauma` — Posoperatorio · Politraumatismo
- `p_cv_cronica` — Posoperatorio · Enfermedad cardiovascular crónica
- `p_vascular` — Posoperatorio · Cirugía vascular periférica
- `p_valva` — Posoperatorio · Cirugía valvular cardíaca
- `p_cranio_neo` — Posoperatorio · Craneotomía por neoplasia
- `p_renal_neo` — Posoperatorio · Cirugía renal por neoplasia
- `p_tx_renal` — Posoperatorio · Trasplante renal
- `p_tce` — Posoperatorio · Traumatismo craneoencefálico
- `p_torax_neo` — Posoperatorio · Cirugía torácica por neoplasia
- `p_cranio_hic` — Posoperatorio · Craneotomía por hemorragia intracraneal, subaracnoidea o subdural
- `p_coluna` — Posoperatorio · Laminectomía o cirugía de médula espinal
- `p_choque` — Posoperatorio · Shock hemorrágico
- `p_hda` — Posoperatorio · Hemorragia digestiva
- `p_gi_neo` — Posoperatorio · Cirugía gastrointestinal por neoplasia
- `p_insuf_resp` — Posoperatorio · Insuficiencia respiratoria tras cirugía
- `p_perfuracao` — Posoperatorio · Perforación u obstrucción gastrointestinal
- `p_outro_neuro` — Posoperatorio · Otro: neurológico
- `p_outro_cv` — Posoperatorio · Otro: cardiovascular
- `p_outro_resp` — Posoperatorio · Otro: respiratorio
- `p_outro_gi` — Posoperatorio · Otro: gastrointestinal
- `p_outro_metab` — Posoperatorio · Otro: metabólico o renal

## Edición del método

APACHE II/Knaus 1985: 12 variables; edad; enfermedad crónica; oxigenación por FiO₂; modelo logístico diagnóstico

## Fórmula documentada

APACHE II = puntuación fisiológica aguda (12 variables, 0 a 4 puntos cada una; Glasgow aporta 15 − Glasgow) + puntos por edad (≤ 44 = 0; 45–54 = 2; 55–64 = 3; 65–74 = 5; ≥ 75 = 6) + enfermedad crónica (5 puntos en ingreso médico o posoperatorio urgente; 2 puntos en posoperatorio electivo).

Oxigenación: con FiO₂ ≥ 50%, puntúe el gradiente A–a \[FiO₂ × 713 − PaCO₂/0,8 − PaO₂\]: ≥ 500 = 4; 350–499 = 3; 200–349 = 2; \< 200 = 0. Con FiO₂ \< 50%, puntúe PaO₂: \> 70 = 0; 61–70 = 1; 55–60 = 3; \< 55 = 4. Los puntos por creatinina se duplican en insuficiencia renal aguda.

Mortalidad hospitalaria prevista: ln\[R/(1 − R)\] = −3,517 + 0,146 × APACHE II + 0,603 (si cirugía urgente) + peso de la categoría diagnóstica.

## Límites y población

El APACHE II de 1985 se relacionó con la mortalidad hospitalaria en 5815 ingresos en UCI de 13 hospitales. La estratificación pronóstica descrita por los autores combina la puntuación con una descripción precisa de la enfermedad; el total aislado no reproduce esa información diagnóstica. La ventana de recogida, las exclusiones y la aplicabilidad fuera de esta población deben comprobarse en el método completo.

## Referencias

- [Knaus WA, Draper EA, Wagner DP, Zimmerman JE. APACHE II: a severity of disease classification system. Crit Care Med, 1985.](https://doi.org/10.1097/00003246-198510000-00009)

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
