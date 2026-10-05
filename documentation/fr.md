<!-- ELUCENIA technical documentation · apache-ii · fr · no clinical/professional/rights approval -->

# APACHE II

[conditions, sources et autorisations](https://elucenia.org/fr/outils/apache-ii)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Âge

`idade`

ans · intervalle: 16–110

### Température centrale

`temp`

°C · intervalle: 25–45

### Pression artérielle moyenne

`pam`

mmHg · intervalle: 20–250

### Fréquence cardiaque

`fc`

bpm · intervalle: 20–250

### Fréquence respiratoire

`fr`

respirations/min · intervalle: 0–80

### FiO₂

`fio2`

% · intervalle: 21–100

### PaO₂

`pao2`

mmHg · intervalle: 20–700

### PaCO₂ (nécessaire si FiO₂ ≥ 50 %)

`paco2`

mmHg · facultatif · intervalle: 10–150

### pH artériel

`ph`

intervalle: 6,5–8

### Sodium

`na`

mEq/L · intervalle: 90–200

### Potassium

`k`

mEq/L · intervalle: 1–10

### Créatinine

`cr`

mg/dL · intervalle: 0,1–20

### Insuffisance rénale aiguë ?

`ira`

- `0` — Non
- `1` — Oui

### Hématocrite

`ht`

% · intervalle: 5–75

### Leucocytes

`leuco`

×10³/µL · intervalle: 0,1–200

### Échelle de coma de Glasgow

`gcs`

intervalle: 3–15

### Défaillance viscérale grave préexistante ou immunodépression (cirrhose, NYHA IV, BPCO sévère, dialyse chronique, immunodépression)

`cronica`

- `0` — Non
- `1` — Oui

### Type d’admission

`admissao`

- `clin` — Médicale (non chirurgicale)
- `urg` — Après chirurgie en urgence
- `elet` — Après chirurgie programmée

### Catégorie diagnostique principale

`diag`

- `n_asma` — Médical · Insuffisance respiratoire : asthme ou allergie
- `n_dpoc` — Médical · Insuffisance respiratoire : BPCO
- `n_edema` — Médical · Insuffisance respiratoire : œdème pulmonaire non cardiogénique
- `n_pcr_resp` — Médical · Insuffisance respiratoire : après arrêt respiratoire
- `n_aspiracao` — Médical · Insuffisance respiratoire : inhalation, intoxication ou exposition toxique
- `n_tep` — Médical · Insuffisance respiratoire : embolie pulmonaire
- `n_infec_resp` — Médical · Insuffisance respiratoire : infection
- `n_neo_resp` — Médical · Insuffisance respiratoire : néoplasie
- `n_has` — Médical · Cardiovasculaire : hypertension
- `n_ritmo` — Médical · Cardiovasculaire : trouble du rythme
- `n_icc` — Médical · Cardiovasculaire : insuffisance cardiaque congestive
- `n_hipovol` — Médical · Cardiovasculaire : choc hémorragique ou hypovolémie
- `n_dac` — Médical · Cardiovasculaire : maladie coronarienne
- `n_sepse` — Sepsis (médical ou postopératoire)
- `n_pcr` — Après arrêt cardiaque (médical ou postopératoire)
- `n_cardiog` — Médical · Cardiovasculaire : choc cardiogénique
- `n_aneur` — Médical · Cardiovasculaire : dissection ou anévrisme aortique
- `n_politrauma` — Médical · Traumatisme : polytraumatisme
- `n_tce` — Médical · Traumatisme : traumatisme crânien
- `n_convulsao` — Médical · Neurologique : crise convulsive
- `n_hic` — Médical · Neurologique : hémorragie intracrânienne, hémorragie sous-arachnoïdienne ou hématome sous-dural
- `n_intox` — Médical · Surdosage médicamenteux ou de drogues
- `n_cad` — Médical · Acidocétose diabétique
- `n_hda` — Médical · Hémorragie digestive
- `n_outro_metab` — Médical · Autre : métabolique ou rénal
- `n_outro_resp` — Médical · Autre : respiratoire
- `n_outro_neuro` — Médical · Autre : neurologique
- `n_outro_cv` — Médical · Autre : cardiovasculaire
- `n_outro_gi` — Médical · Autre : gastro-intestinal
- `p_politrauma` — Postopératoire · Polytraumatisme
- `p_cv_cronica` — Postopératoire · Maladie cardiovasculaire chronique
- `p_vascular` — Postopératoire · Chirurgie vasculaire périphérique
- `p_valva` — Postopératoire · Chirurgie valvulaire cardiaque
- `p_cranio_neo` — Postopératoire · Craniotomie pour néoplasie
- `p_renal_neo` — Postopératoire · Chirurgie rénale pour néoplasie
- `p_tx_renal` — Postopératoire · Transplantation rénale
- `p_tce` — Postopératoire · Traumatisme crânio-encéphalique
- `p_torax_neo` — Postopératoire · Chirurgie thoracique pour néoplasie
- `p_cranio_hic` — Postopératoire · Craniotomie pour hémorragie intracrânienne, sous-arachnoïdienne ou sous-durale
- `p_coluna` — Postopératoire · Laminectomie ou chirurgie médullaire
- `p_choque` — Postopératoire · Choc hémorragique
- `p_hda` — Postopératoire · Hémorragie digestive
- `p_gi_neo` — Postopératoire · Chirurgie gastro-intestinale pour néoplasie
- `p_insuf_resp` — Postopératoire · Insuffisance respiratoire après chirurgie
- `p_perfuracao` — Postopératoire · Perforation ou occlusion gastro-intestinale
- `p_outro_neuro` — Postopératoire · Autre : neurologique
- `p_outro_cv` — Postopératoire · Autre : cardiovasculaire
- `p_outro_resp` — Postopératoire · Autre : respiratoire
- `p_outro_gi` — Postopératoire · Autre : gastro-intestinal
- `p_outro_metab` — Postopératoire · Autre : métabolique ou rénal

## Édition de la méthode

APACHE II/Knaus 1985 : 12 variables ; âge ; maladie chronique ; oxygénation selon FiO₂ ; modèle logistique diagnostique

## Formule documentée

APACHE II = score physiologique aigu (12 variables, 0 à 4 points chacune ; Glasgow contribue 15 − Glasgow) + points d’âge (≤ 44 = 0; 45–54 = 2; 55–64 = 3; 65–74 = 5; ≥ 75 = 6) + maladie chronique (5 points en admission médicale ou après chirurgie urgente ; 2 après chirurgie programmée).

Oxygénation : avec FiO₂ ≥ 50%, noter le gradient A–a \[FiO₂ × 713 − PaCO₂/0,8 − PaO₂\]: ≥ 500 = 4; 350–499 = 3; 200–349 = 2; \< 200 = 0. Avec FiO₂ \< 50%, noter PaO₂ : \> 70 = 0; 61–70 = 1; 55–60 = 3; \< 55 = 4. Les points de créatinine sont doublés en cas d’insuffisance rénale aiguë.

Mortalité hospitalière prédite : ln\[R/(1 − R)\] = −3,517 + 0,146 × APACHE II + 0,603 (si chirurgie urgente) + poids de la catégorie diagnostique.

## Limites et population

L’APACHE II de 1985 a été associé à la mortalité hospitalière dans 5815 admissions en réanimation dans 13 hôpitaux. La stratification pronostique décrite par les auteurs combine le score avec une description précise de la maladie ; le total seul ne reproduit pas cette information diagnostique. La fenêtre de recueil, les exclusions et l’applicabilité hors de cette population doivent être vérifiées dans la méthode intégrale.

## Références

- [Knaus WA, Draper EA, Wagner DP, Zimmerman JE. APACHE II: a severity of disease classification system. Crit Care Med, 1985.](https://doi.org/10.1097/00003246-198510000-00009)

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
