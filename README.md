# Prediction-sinistres

Projet : Prévision des Sinistres à partir d'une Série Chronologique

Ce projet consiste à analyser et modéliser une série chronologique des sinistres enregistrés dans un contexte d’assurance. L'objectif principal est de comprendre les tendances passées et d'utiliser ces modèles pour prédire les sinistres futurs.

Objectifs

Analyse descriptive : Explorer la série chronologique pour identifier les tendances principales.

Division des données : Séparer les données en ensemble d’entraînement et de test pour une validation robuste.

Prévision : Utiliser des modèles ARIMA et GARCH pour modéliser et prédire les sinistres futurs.

Données

Le projet repose sur un fichier .Rdata contenant les relevés de sinistres.

Nom de l’objet : Sinistres.

Variables principales :

Dates : Points de temps de la série.

Sinistres : Nombre ou montant des sinistres enregistrés.

Méthodologie

1. Analyse descriptive

Visualisation :

Utilisation de graphiques temporels pour observer les évolutions des sinistres.

Histogrammes pour analyser la distribution.

2. Division des données

Séparation des données :

Ensemble d’entraînement : Les n-h premières observations.

Ensemble de test : Les h dernières observations (validation).

Transformation des données en objets ts (série temporelle).

3. Modélisation et prévision

Modèles utilisés :

Modèles ARIMA (Auto-Regressive Integrated Moving Average).

Modèles GARCH (Generalized Autoregressive Conditional Heteroskedasticity) pour capturer la volatilité.

Validation : Comparaison des prédictions avec les valeurs réelles de l’ensemble de test.

Outils et Bibliothèques

Le projet est réalisé avec les bibliothèques R suivantes :

tseries : Modélisation des séries chronologiques.

rugarch : Modèles GARCH pour analyser la volatilité.

tidyverse : Manipulation et visualisation des données.

reshape2 : Restructuration des données pour l’analyse.

Installation des packages nécessaires :

install.packages(c("tseries", "rugarch", "tidyverse", "reshape2"))

Structure du Projet

Importation des données : Chargement de l’objet Sinistres depuis un fichier .Rdata.

Analyse descriptive : Exploration statistique et visuelle des données.

Division des données : Séparation en ensemble d’entraînement et de test.

Modélisation : Construction des modèles ARIMA et GARCH.

Prévision : Comparaison des résultats prédits avec les valeurs réelles.

