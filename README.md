# Projet : Challenge - Risque de Marché Banque de France

Ce projet a été conçu pour répondre à un défi lié à l’analyse du risque de marché, en mettant en œuvre des méthodologies quantitatives et des outils d’analyse de données. Il s’articule autour de plusieurs étapes principales visant à extraire des informations clés à partir de données financières.

## Fonctionnalités principales

### 1. Reconstitution des données manquantes
Le projet utilise des techniques avancées pour traiter les données incomplètes, en reconstituant les valeurs manquantes afin de garantir une analyse précise et fiable.

### 2. Importation des fichiers Excel
Des fichiers de données financiers sont importés et analysés pour identifier les colonnes pertinentes. Ces fichiers contiennent notamment des informations sur les obligations.

### 3. Filtrage et fusion des jeux de données
- Les obligations sont filtrées en fonction de critères comme le volume (supérieur à $10^{12}$) et le risque (évalué à "LOW").
- Plusieurs jeux de données sont fusionnés pour produire une base consolidée.

## Challenge Description

Votre supérieur vous communique deux fichiers au format Excel contenant :

- Des données sur des obligations.
- Un historique de performance d’un des portefeuilles actuellement sous gestion.

Cependant, certaines données d’un des fichiers ont été corrompues puis supprimées.

### Votre mission est la suivante :

#### Partie 1 : Reconstitution des données manquantes

Reconstituez les données manquantes dans le tableau descriptif tel qu’il apparaît dans le fichier ‘Bonds_Risk_Perf’, en appliquant les critères suivants :

- Inclure uniquement les obligations pour lesquelles :
  - Le volume est supérieur à $10^{12}$.
  - La catégorie de risque `ISSUER_RISK_CAT` est ‘LOW’.

Une fois les données complétées, réalisez une représentation graphique de la courbe de taux des obligations selon leur pays. Commentez :

- La forme de la courbe de taux.
- Les différences de cette courbe entre les différents pays.

#### Partie 2 : Analyse de la performance du portefeuille

Dans l’onglet `Ptf` du fichier ‘Bond_Risk_Perf’, réalisez les analyses suivantes :

1. Représentez graphiquement l’évolution de la valeur du portefeuille via un indice base 100.
2. Avec une fenêtre glissante sur 1 mois, calculez et représentez graphiquement :
   - Value at Risk (VaR) paramétrique au niveau de confiance 99%.
   - Expected Shortfall (ES) historique au niveau de confiance 95%.
3. Représentez graphiquement la distribution des rendements quotidiens.
4. Laquelle des deux métriques vous paraît la plus pertinente ? Justifiez votre réponse.

#### Partie 3 : Calcul des métriques de synthèse

Dans un tableau synthétique, calculez les métriques suivantes sur le portefeuille :

- Le rendement quotidien moyen et médian.
- Le Sharpe ratio (en utilisant le taux ESTER comme taux sans risque).
- Le maximum drawdown (Max Drawdown).

## Technologies utilisées
- **Python** : Langage principal pour le traitement et l’analyse des données.
- **Bibliothèques** : Pandas pour la manipulation des données, Matplotlib/Seaborn pour la visualisation.


## Structure des fichiers
- **Code_BDF_Callenge - Nathan FLEURY.ipynb** : Notebook principal contenant le code et les analyses.
- **Report - Nathan FLEURY.pdf** : Rapport final qui adresse les questions posées et explique les résultats obtenus grâce à l'analyse.
