<!-- ELUCENIA technical documentation · apache-ii · pt-BR · no clinical/professional/rights approval -->

# APACHE II

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/apache-ii)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Idade

`idade`

anos · intervalo: 16–110

### Temperatura central

`temp`

°C · intervalo: 25–45

### Pressão arterial média

`pam`

mmHg · intervalo: 20–250

### Frequência cardíaca

`fc`

bpm · intervalo: 20–250

### Frequência respiratória

`fr`

irpm · intervalo: 0–80

### FiO₂

`fio2`

% · intervalo: 21–100

### PaO₂

`pao2`

mmHg · intervalo: 20–700

### PaCO₂ (necessária se FiO₂ ≥ 50%)

`paco2`

mmHg · opcional · intervalo: 10–150

### pH arterial

`ph`

intervalo: 6,5–8

### Sódio

`na`

mEq/L · intervalo: 90–200

### Potássio

`k`

mEq/L · intervalo: 1–10

### Creatinina

`cr`

mg/dL · intervalo: 0,1–20

### Insuficiência renal aguda?

`ira`

- `0` — Não
- `1` — Sim

### Hematócrito

`ht`

% · intervalo: 5–75

### Leucócitos

`leuco`

×10³/µL · intervalo: 0,1–200

### Escala de Coma de Glasgow

`gcs`

intervalo: 3–15

### Insuficiência orgânica grave prévia ou imunossupressão (cirrose, NYHA IV, DPOC grave, diálise crônica, imunossupressão)

`cronica`

- `0` — Não
- `1` — Sim

### Tipo de admissão

`admissao`

- `clin` — Clínica (não cirúrgica)
- `urg` — Pós-operatório de urgência
- `elet` — Pós-operatório eletivo

### Categoria diagnóstica principal

`diag`

- `n_asma` — Clínico · Insuf. respiratória: asma ou alergia
- `n_dpoc` — Clínico · Insuf. respiratória: DPOC
- `n_edema` — Clínico · Insuf. respiratória: edema pulmonar não cardiogênico
- `n_pcr_resp` — Clínico · Insuf. respiratória: pós-parada respiratória
- `n_aspiracao` — Clínico · Insuf. respiratória: aspiração, intoxicação ou tóxico
- `n_tep` — Clínico · Insuf. respiratória: embolia pulmonar
- `n_infec_resp` — Clínico · Insuf. respiratória: infecção
- `n_neo_resp` — Clínico · Insuf. respiratória: neoplasia
- `n_has` — Clínico · Cardiovascular: hipertensão
- `n_ritmo` — Clínico · Cardiovascular: distúrbio do ritmo
- `n_icc` — Clínico · Cardiovascular: insuficiência cardíaca congestiva
- `n_hipovol` — Clínico · Cardiovascular: choque hemorrágico ou hipovolemia
- `n_dac` — Clínico · Cardiovascular: doença arterial coronariana
- `n_sepse` — Sepse (clínico ou pós-operatório)
- `n_pcr` — Pós-parada cardíaca (clínico ou pós-operatório)
- `n_cardiog` — Clínico · Cardiovascular: choque cardiogênico
- `n_aneur` — Clínico · Cardiovascular: dissecção ou aneurisma de aorta
- `n_politrauma` — Clínico · Trauma: politrauma
- `n_tce` — Clínico · Trauma: trauma cranioencefálico
- `n_convulsao` — Clínico · Neurológico: crise convulsiva
- `n_hic` — Clínico · Neurológico: hemorragia intracraniana, HSA ou hematoma subdural
- `n_intox` — Clínico · Overdose de drogas
- `n_cad` — Clínico · Cetoacidose diabética
- `n_hda` — Clínico · Hemorragia digestiva
- `n_outro_metab` — Clínico · Outro: metabólico ou renal
- `n_outro_resp` — Clínico · Outro: respiratório
- `n_outro_neuro` — Clínico · Outro: neurológico
- `n_outro_cv` — Clínico · Outro: cardiovascular
- `n_outro_gi` — Clínico · Outro: gastrointestinal
- `p_politrauma` — Pós-operatório · Politrauma
- `p_cv_cronica` — Pós-operatório · Doença cardiovascular crônica
- `p_vascular` — Pós-operatório · Cirurgia vascular periférica
- `p_valva` — Pós-operatório · Cirurgia valvar
- `p_cranio_neo` — Pós-operatório · Craniotomia por neoplasia
- `p_renal_neo` — Pós-operatório · Cirurgia renal por neoplasia
- `p_tx_renal` — Pós-operatório · Transplante renal
- `p_tce` — Pós-operatório · Trauma cranioencefálico
- `p_torax_neo` — Pós-operatório · Cirurgia torácica por neoplasia
- `p_cranio_hic` — Pós-operatório · Craniotomia por hemorragia intracraniana, HSA ou subdural
- `p_coluna` — Pós-operatório · Laminectomia ou cirurgia medular
- `p_choque` — Pós-operatório · Choque hemorrágico
- `p_hda` — Pós-operatório · Hemorragia digestiva
- `p_gi_neo` — Pós-operatório · Cirurgia gastrointestinal por neoplasia
- `p_insuf_resp` — Pós-operatório · Insuficiência respiratória após cirurgia
- `p_perfuracao` — Pós-operatório · Perfuração ou obstrução gastrointestinal
- `p_outro_neuro` — Pós-operatório · Outro: neurológico
- `p_outro_cv` — Pós-operatório · Outro: cardiovascular
- `p_outro_resp` — Pós-operatório · Outro: respiratório
- `p_outro_gi` — Pós-operatório · Outro: gastrointestinal
- `p_outro_metab` — Pós-operatório · Outro: metabólico ou renal

## Edição do método

APACHEII/Knaus 1985:12 variáveis; idade; doença crônica; oxigenação por Fi O 2; modelo logístico diagnóstico

## Fórmula documentada

APACHE II = escore fisiológico agudo (12 variáveis, 0 a 4 pontos cada; Glasgow entra como 15 − Glasgow) + pontos de idade (≤ 44 = 0; 45–54 = 2; 55–64 = 3; 65–74 = 5; ≥ 75 = 6) + doença crônica (5 pontos em admissão clínica ou pós-operatório de urgência; 2 pontos no pós-operatório eletivo).

Oxigenação: com FiO₂ ≥ 50%, pontua o gradiente A-a \[FiO₂ × 713 − PaCO₂/0,8 − PaO₂\]: ≥ 500 = 4; 350–499 = 3; 200–349 = 2; \< 200 = 0. Com FiO₂ \< 50%, pontua a PaO₂: \> 70 = 0; 61–70 = 1; 55–60 = 3; \< 55 = 4. A creatinina tem pontos dobrados na insuficiência renal aguda.

Mortalidade hospitalar prevista: ln\[R/(1 − R)\] = −3,517 + 0,146 × APACHE II + 0,603 (se cirurgia de urgência) + peso da categoria diagnóstica.

## Limites e população

O APACHE II de 1985 foi relacionado à mortalidade hospitalar em 5815 admissões em UTI de 13 hospitais. A estratificação prognóstica descrita pelos autores combina o escore com uma descrição precisa da doença; o total isolado não reproduz essa informação diagnóstica. A janela de coleta, as exclusões e a aplicabilidade fora dessa população precisam de conferência no método integral.

## Referências

- [Knaus WA, Draper EA, Wagner DP, Zimmerman JE. APACHE II: a severity of disease classification system. Crit Care Med, 1985.](https://doi.org/10.1097/00003246-198510000-00009)

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
