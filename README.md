# Modélisation ML - test technique

Ce dépôt contient une analyse approfondie des données du dataset test_technique_dataset.xlsx en utilisant le modèle XGBoost pour la classification.

## Description de l'analyse

L'analyse a été divisée en plusieurs étapes clés:

### 1. Exploration des données
- Chargement du jeu de données à partir d'une source externe.
- Exploration initiale pour comprendre la structure, les types de données et les premières statistiques descriptives.
### 2. Prétraitement des données 
- Traitement des valeurs manquantes et des anomalies.
- Encodage des variables catégorielles et normalisation des variables continues.
### 3. Choix du modèle 
- XGBoost a été privilégié pour sa capacité à fournir de meilleures performances avec moins de temps d'entraînement.
- Il est robuste face aux valeurs manquantes et est performant pour les grands jeux de données.
### 4. Équilibrage des données 
- En raison de la répartition inégale des classes, la technique SMOTE a été utilisée pour équilibrer les données avant l'entraînement.
### 5. Entraînement du modèle 
- Entraînement du modèle XGBoost avec les paramètres optimaux.
### 6. Évaluation 
- Évaluation des performances à l'aide de la matrice de confusion, de la courbe ROC et d'autres métriques pertinentes.
### 7. Sauvegarde des résultats 
- Les prédictions ont été sauvegardées dans 'prediction.csv' et la matrice de confusion dans 'confusion_matrix.csv'.


## Comment lancer l'analyse
Pour reproduire l'analyse, vous devez suivre ces étapes:

### 1. Cloner le dépot 

git clone https://github.com/NAMSAGUINE/NAMSAGUINE?search=1
cd NAMSAGUINE

### 2. Environnement virtuel (optionnel mais recommandé)
python3 -m venv mon_env
source mon_env/bin/activate

### 3. Installer les dépendances
pip install -r requirements.txt

### 4. Lancer le notebook 
jupyter notebook 
- Ouvrez le notebook test-technique-AMAGUINE.ipynb et exécutez toutes les cellules.
### 5. Conversion du notebook en script Python  (optionnel)
jupyter nbconvert --to script test-technique-AMAGUINE.ipynb
python test-technique-AMAGUINE.py

- Si vous préférez exécuter le notebook sous forme de script, vous pouvez le convertir en un fichier .py et l'exécuter.

### 6. Consultation des résultats

Après avoir exécuté l'analyse, vous devriez voir les fichiers prediction.csv et confusion_matrix.csv générés dans le répertoire courant. Ces fichiers contiennent les prédictions du modèle et la matrice de confusion, respectivement.








