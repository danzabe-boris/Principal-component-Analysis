# Principal-component-Analysis
# Readme

## Forage de Données

Ce code effectue des opérations de forage de données pour prédire la classe d'un jeu de données en utilisant l'algorithme K-NN et l'algorithme SVM. 

## Importation des bibliothéques

Le code utilise les bibliothèques suivantes:
* scikit-learn (sklearn) - pour la mise en œuvre des algorithmes de classification
* numpy (np) - pour la manipulation de tableaux
* scipy (sp) - pour les opérations mathématiques
* seaborn (sns) - pour la visualisation de données
* pandas (pd) - pour la manipulation de données en tableau
* matplotlib.pyplot (plt) - pour la visualisation de graphiques
* warnings - pour ignorer les avertissements
* itertools - pour les opérations de produit cartésien

## Importation des données

Le code importe les données à partir du fichier csv `TP3_data.csv` et les stocke dans un dataframe appelé `data`.

## Prétraitement des données

Le code standardise les données à l'aide de la fonction StandardScaler() de scikit-learn.

## Implémentation de fonctions

Le code implémente les fonctions suivantes pour l'optimisation des modèles:
* `model_score(X,y,class_model,params)` - pour calculer la précision d'un modèle à l'aide de la validation croisée
* `bruteforce_optimisation(class_model,grille_param,X,y)` - pour trouver les meilleurs hyperparamètres en effectuant une recherche exhaustive de toutes les combinaisons possibles
* `randomize_optimisation(class_model,grille_param,X,y,sample_percent)` - pour trouver les meilleurs hyperparamètres en effectuant une recherche aléatoire
* `halving_optimisation(class_model,grille_param,X,y)` - pour trouver les meilleurs hyperparamètres en effectuant une recherche basée sur le principe de la méthode de "halving".

## Comment exécuter le code

Pour exécuter le code, il suffit d'ouvrir le fichier dans un environnement Python et d'exécuter les cellules une par une. Les résultats seront affichés dans les sorties correspondantes. 

## Conclusion

Le code fournit des fonctions pour optimiser les modèles de classification en utilisant différents algorithmes et en effectuant différentes méthodes d'optimisation. Ces fonctions peuvent être utilisées pour améliorer les performances de classification des modèles de données et pour fournir des prédictions plus précises.
