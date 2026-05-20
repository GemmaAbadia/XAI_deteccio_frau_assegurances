# TFM - Explainable AI per a la detecció de frau en assegurances

Aquest repositori conté el desenvolupament complet del Treball Final de Màster centrat en l’aplicació de tècniques de Machine Learning i Explainable Artificial Intelligence (XAI) per a la detecció de frau en assegurances.

L’objectiu principal del projecte és comparar diferents models predictius, tant interpretables com black-box, i analitzar com tècniques XAI com SHAP i Anchors poden millorar la transparència i interpretabilitat de les prediccions.

---

# Estructura del projecte

```text
projecte_tfm/

│
├── dades/
│   ├── original/
│   └── preprocessades/
│
├── notebooks/
│   ├── 01_preparacio_i_preprocessament_dades.ipynb
│   └── 02_modelatge_predictiu_i_xai.ipynb
│
├── models/
│
├── figures/
│
├── requirements.txt
│
└── README.md
````

---

# Descripció dels directoris

## dades/

Conté els datasets utilitzats durant el projecte.

### original/

Dataset original abans del preprocessament.

### preprocessades/

Datasets transformats i preparats per al modelatge.

---

## notebooks/

### 01_preparacio_i_preprocessament_dades.ipynb

Notebook dedicat a:

* anàlisi inicial del dataset,
* tractament de valors nuls i valors especials,
* enginyeria de característiques,
* transformacions temporals,
* reducció i selecció de variables,
* codificació de variables categòriques,
* partició train/test,
* preparació final per al modelatge.

---

### 02_modelatge_predictiu_i_xai.ipynb

Notebook principal del projecte.

Inclou:

* entrenament de models baseline:

  * regressió logística,
  * arbre de decisió,
* entrenament de models black-box:

  * Random Forest,
  * XGBoost,
  * SVC,
  * MLP,
* optimització d’hiperparàmetres,
* threshold tuning,
* avaluació de mètriques,
* comparació de models,
* aplicació de SHAP,
* aplicació d’Anchors,
* interpretació de resultats XAI.

---

## models/

Directori reservat per guardar:

* models entrenats,
* escaladors,
* objectes serialitzats (`joblib`, `pickle`, etc.),
* configuracions finals.

---

## figures/

Directori reservat per emmagatzemar:

* ROC curves,
* confusion matrices,
* gràfiques de threshold tuning,
* SHAP summary plots,
* waterfall plots,
* training curves,
* figures addicionals utilitzades a la memòria.

---

# Reproducció de l’entorn

## Instal·lació de dependències

```bash
pip install -r requirements.txt
```

---

# Principals llibreries utilitzades

* pandas
* numpy
* scikit-learn
* xgboost
* torch
* shap
* alibi
* matplotlib
* seaborn

---

# Reproduïbilitat

Per afavorir la reproduïbilitat:

* s’utilitzen llavors aleatòries fixes (`seed = 42`),
* la separació train/test és estratificada,
* els notebooks segueixen un ordre seqüencial d’execució.

---

# Tècniques XAI utilitzades

## SHAP

Utilitzat per:

* explicacions globals,
* importància de variables,
* explicacions locals,
* waterfall plots.

## Anchors

Utilitzat per:

* generació de regles interpretables,
* explicacions locals basades en condicions lògiques,
* anàlisi de precision i coverage.

---

# Autor

Treball Final de Màster (TFM)

Màster en Ciència de Dades / Intel·ligència Artificial

```
```
