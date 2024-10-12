

# **Financial-Analysis-of-the-Moroccan-Government-2004-2023**

## **1. Objectif du Projet**
Ce projet vise à analyser et prévoir les données financières du gouvernement marocain de 2004 à 2023. Les prévisions sont effectuées à l'aide de divers modèles de séries temporelles : **ARIMA**, **VAR**, **LSTM**, ainsi que la détection des anomalies avec **Isolation Forest**.

## **2. Données Utilisées**
Le projet repose sur des données financières comprenant :
- **IS** : Impôt sur les sociétés
- **IR** : Impôt sur le revenu
- **TVA** : Taxe sur la valeur ajoutée
- **TIC** : Taxe intérieure de consommation
- **BetS** : Dépenses en biens et services
- **intD** : Intérêt de la dette
- **COMP** : Compensation

Les données sont enrichies par la création de nouvelles colonnes pour le **total des recettes mensuelles** et les **dépenses mensuelles**.

## **3. Bibliothèques Utilisées**

Le projet utilise les bibliothèques suivantes :

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.ensemble import IsolationForest
from statsmodels.tsa.api import VAR
from statsmodels.tsa.arima.model import ARIMA
from sklearn.metrics import mean_squared_error, mean_absolute_percentage_error
from sklearn.linear_model import LinearRegression
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import LSTM, Dense
from sklearn.preprocessing import MinMaxScaler
from statsmodels.tsa.stattools import adfuller
from statsmodels.stats.stattools import jarque_bera
from statsmodels.stats.diagnostic import acorr_ljungbox
import warnings
```

## **4. Architecture du Projet**

### **Étapes Principales :**
1. **Préparation des données** : 
   - Chargement des données depuis un fichier Excel.
   - Nettoyage et transformation (formatage des dates, ajout de colonnes calculées).
   
2. **Modélisation** :
   - **ARIMA** : Pour les prévisions univariées des séries temporelles.
   - **VAR** : Pour modéliser les relations entre plusieurs variables.
   - **LSTM** : Utilisation de réseaux de neurones récurrents pour capturer les tendances non linéaires.
   - **SARIMA** : Pour les prévisions univariées des séries temporelles saisonnières.
   - **Isolation Forest** : Détection des anomalies dans les données financières.

3. **Évaluation** :
   - Utilisation de métriques telles que **RMSE** (Root Mean Squared Error) et **MAPE** (Mean Absolute Percentage Error) pour évaluer la performance des modèles.

4. **Détection des Anomalies** :
   - Identification des irrégularités dans les données à l'aide du modèle **Isolation Forest**.

## **5. Résultats**
- **Prévisions** : Les modèles ARIMA, VAR et LSTM fournissent des prévisions des recettes et des dépenses mensuelles.
- **Anomalies** : Les anomalies dans les données financières sont détectées, permettant d'améliorer la gestion des risques.

## **6. Comment Utiliser ce Projet**
1. Clone ce repository :
   ```bash
   git clone https://github.com/ton-repository/Financial-Analysis-of-the-Moroccan-Government-2004-2023.git
   cd Financial-Analysis-of-the-Moroccan-Government-2004-2023
   ```

2. Installe les dépendances requises (via `requirements.txt`) :
   ```bash
   pip install -r requirements.txt
   ```

3. Lance le notebook pour exécuter l'analyse et les prévisions :
   ```bash
   jupyter notebook
   ```

## **7. Structure des Fichiers**
- `notebooks/`: Contient les notebooks Jupyter pour l'analyse et les prévisions.
- `data/`: Contient les jeux de données utilisés.
- `requirements.txt`: Liste des bibliothèques nécessaires pour le projet.

## **8. Technologies Utilisées**
- **Python** : Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, TensorFlow,statsmodel
- **Modèles de prévision** : ARIMA, VAR, LSTM,SARIMA
- **Détection d'anomalies** : Isolation Forest
- **Jupyter Notebook** : Pour la visualisation et l'analyse

## **9. Contributeurs**
- Moussaab : Créateur et développeur du projet.

