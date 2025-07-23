# Mémoire de M1 – Analyse de l'optimisation des dépenses en R&D aux US à l'ère de l'IA 

Ce dépôt regroupe l'ensemble des données, du notebook Python et du document PDF utilisés pour la rédaction d'un mémoire de Master 1. L'étude s'intéresse à Analyse de l'optimisation des dépenses en R&D aux US à l'ère de l'IA notamment au travers des dépenses de recherche et développement (DIRD) aux États‑Unis ainsi qu'à la dynamique des brevets liés à l'intelligence artificielle.

## Contenu du dépôt

| Fichier | Description |
| --- | --- |
| `Donnees_mémoire_traitement (2).ipynb` | Notebook principal de traitement des données et de modélisation. On y retrouve l'imputation des valeurs manquantes par KNN, le calcul de plusieurs indicateurs (Lorenz, Gini, HHI), ainsi que des modèles OLS et SARIMAX. |
| `Données_memoire.xlsx` | Jeu de données de base. Il comprend notamment les variables de dépenses de R&D par secteur, le PIB, les dépenses fédérales et différentes mesures liées aux brevets IA. |
| `df1.xlsx` | Jeu de données préparé pour l'analyse chronologique (1974‑2023). |
| `Memo_US.pdf` | Version PDF du mémoire (document _doc_memo_). |

## Utilisation rapide

1. Ouvrir le notebook Jupyter pour reproduire les traitements (nécessite les bibliothèques `numpy`, `pandas`, `statsmodels`, etc.).
2. Les fichiers Excel contiennent les séries temporelles utilisées dans l'étude. La feuille `sheet1` de `Données_memoire.xlsx` comprend par exemple les colonnes :
   - Années
   - DIRD total et par secteur
   - PIB (GDP)
   - Demande et offre de brevets, dont les brevets IA (D et O)
   - Cycle time to market des brevets
   - Soutien public via le crédit budgétaire et le crédit d'impôt recherche
3. Le fichier `Memo_US.pdf` présente l'intégralité de l'analyse rédigée.

## Aperçu de l'analyse

Le notebook suit plusieurs étapes :

- **Analyse des valeurs manquantes** : détection et imputation par KNN.
- **Construction d'indicateurs** : productivité de l'IA, intensité DIRD/PIB, soutien public, etc.
- **Mesure de la concentration** : courbes de Lorenz, indices de Gini et HHI.
- **Modélisation** : régressions OLS et modèles SARIMAX pour expliquer la dynamique des dépenses et des brevets.

## Licence

Les données proviennent principalement de l'OCDE et d'organismes publics américains. Le code et la documentation de ce dépôt sont mis à disposition sans garantie.
