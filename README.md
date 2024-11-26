# Aperçu du Projet
Ce projet se concentre sur l'analyse et la prédiction des coûts d'assurance à l'aide de techniques d'apprentissage automatique. Il inclut le prétraitement des données, l'analyse exploratoire et l'entraînement de modèles, avec des sorties sauvegardées pour assurer la reproductibilité.

## Structure du Projet

### 1. Configuration et Métadonnées
- **`.gitignore`** : Spécifie les fichiers et dossiers à exclure du contrôle de version.
- **`README.md`** : Documentation du projet (vous y êtes !).
- **`requirements.txt`** : Liste des dépendances Python nécessaires pour exécuter le projet.

### 2. Données
- **`data/raw/insurance.csv`** : Jeu de données brut contenant les données d'assurance originales.
- **`data/process/insurance_clean.csv`** : Jeu de données nettoyé après prétraitement.

### 3. Notebooks
- **`notebook/exploration.ipynb`** : Notebook pour l'analyse exploratoire, y compris l'analyse de distribution et de corrélation.
- **`notebook/pretraitement.ipynb`** : Notebook pour le prétraitement des données, y compris la gestion des valeurs manquantes et des outliers.
- **`notebook/training.ipynb`** : Notebook pour l'entraînement des modèles d'apprentissage automatique et l'évaluation de leur performance.

### 4. Résultats
#### Fichiers Pickle
- **`output/pickle/columns.pkl`** : Fichier sérialisé contenant les noms des colonnes utilisées dans le modèle.
- **`output/pickle/encoders.pkl`** : Encodeurs utilisés pour la transformation des données catégoriques.
- **`output/pickle/model.pkl`** : Modèle d'apprentissage automatique entraîné.

#### Graphiques
Visualisations générées pendant l'analyse :
- **`output/plot/bmi_outlier_deleted.png`** : Données de l'IMC après suppression des outliers.
- **`output/plot/distribution_caracteristique.png`** : Distribution des caractéristiques principales.
- **`output/plot/expenses_outlier_transformation.png`** : Données des dépenses transformées après traitement des outliers.
- **`output/plot/matrice_correlation.png`** : Matrice de corrélation du jeu de données.
- **`output/plot/outlier.png`** : Identification des outliers.
- **`output/plot/relation_caracteristique_cible.png`** : Relation entre les caractéristiques et la variable cible.
- **`output/plot/résidus.png`** : Analyse des résidus pour le modèle.
- **`output/plot/transformation_log_expenses.png`** : Transformation logarithmique des dépenses.

## Comment Exécuter le Projet

### Prérequis
1. Installer Python 3.8+.
2. Installer les dépendances nécessaires avec la commande suivante :
   ```bash
   pip install -r requirements.txt
   ```

### Étapes
1. **Explorer les Données** :
   Ouvrir et exécuter `notebook/exploration.ipynb` pour analyser les données brutes.

2. **Prétraiter les Données** :
   Exécuter `notebook/pretraitement.ipynb` pour nettoyer et prétraiter les données.

3. **Entraîner le Modèle** :
   Exécuter `notebook/training.ipynb` pour entraîner le modèle d'apprentissage automatique et générer des prédictions.

4. **Vérifier les Résultats** :
   Inspecter le dossier `output/pickle/` pour les modèles et encodeurs sérialisés. Les visualisations sont sauvegardées dans le répertoire `output/plot/`.

## Fonctionnalités Clés
- Nettoyage et prétraitement des données automatisés.
- Visualisations pour comprendre les caractéristiques des données.
- Entraînement et évaluation des modèles d'apprentissage automatique.
- Sauvegarde des résultats pour assurer la reproductibilité.

## Licence
[Spécifiez ici la licence de votre projet, par exemple, MIT, Apache 2.0, etc.]

