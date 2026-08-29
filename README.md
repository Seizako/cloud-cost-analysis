# gcp-cloud-cost-analysis

Analyse des coûts de facturation GCP : identifier les principaux postes de
dépense par service et par région, et repérer les ressources qui coûtent cher
mais qui sont peu utilisées (gaspillage cloud potentiel).

## Données

- Source : [GCP Cloud Billing Data](https://www.kaggle.com/datasets/sairamn19/gcp-cloud-billing-data) (Kaggle)
- Fichier brut : `data/raw/gcp_final_approved_dataset.csv`
- Données nettoyées : `data/processed/`

## Organisation

```
data/
  raw/        # dataset d'origine, non modifié
  processed/  # données nettoyées
notebooks/
  01_exploration.ipynb   # premier coup d'œil au dataset
```

## Installation

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```
