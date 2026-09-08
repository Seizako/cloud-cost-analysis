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
  01_exploration.ipynb        # premier coup d'œil au dataset
  02_nettoyage.ipynb          # renommage, dates, contrôles, export du CSV propre
  03_analyse.ipynb            # coûts par service / région, détection de gaspillage
  04_recommandations.ipynb    # économies estimées, plan d'action
  05_analyse_temporelle.ipynb # évolution des coûts dans le temps
  06_efficacite.ipynb         # d'où vient le coût, lien coût / utilisation
```

## Installation

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```
