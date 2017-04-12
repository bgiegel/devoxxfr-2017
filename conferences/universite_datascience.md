Université de la datascience

Ma première conf et surement une de mes préférée. C'est une mini formation au machinelearning et un état de l'art sur le deeplearning. Vraiment très intéressant. A voir absolument si vous vous intéressez au sujet mais que vous n'avez jamais eu le temps de faire de la veille dessus.

Exemple avec Jack et le Titanic. Qui va survivre ?

2 type de problème : supervisé et non supervisé

Supervisé : on connaît les données en entrée ( est ce que Jack va mourir )

Non supervise : on a un cluster de client et on veut les catégorisé pour améliorer l'expérience d'une catégorie d'entre eux

Process :

Analyse des données

Démo avec python notebook. Permet de charger des données à la volée

Box plot : permet de segmenter les résultats en se basant sur la médiane.

Violon plot : utile pour voir la répartition par âge.

Comment gérer les données manquantes ?

- on supprime les donnes manquante. Pas terrible

-  on remplace par 0.. non ça fausse les données.

- on remplace par la médiane ( pas la moyenne !). C'est mieux !

Artificial feature : données rajoutés par calcul pour améliorer les prédictions

Par exemple : prendre la colonne gender et créé 2 colonne mâle et femelle avec 0 ou 1

Pour faire des prédictions à partir des données on a plein d'algorithme.

L'algorithme doit bien coller aux data d'entrée mais doit aussi être capable de prédire l'etat des future données.

Pour entrainer son algo à la prédiction il faut utiliser un partie du jeu de données (30%) pour tester l'algorithme et voir la différence entre la prédiction et le résultat connu.

Exemple de cas dans la vrai vie

- Algo linear pas toujours utile quand nuage de point.

- Svm ; bien mais pas scalable

- Decision tree : bien mais sensible au bruit..

- Random forest :scalable. Pas sensible au bruit. Mais il a beaucoup de paramètres.

Exemple d'algorithme non linéaire : réseau de neurones.

Problème quand on veut trouver des spam par exemple : trop strict ou trop lâche

Les datascientist passe seulement 10% de leur temps à faire du machine learning

Les modèles ne sont pas parfaits.

Besoin d'expert du domaine. Beaucoup de soucis de communication avec ces experts. Peur de se faire remplacer. Peur du changement.

La dataviz c'est très important pour expliquer les modèles.

Les datascientist font de l'exploration. Donc du code jetable pas testé et jeté 90% du temps.

Techniques pour y arriver :

- réduire le périmètre
- éviter le over engineering
- les techno de machine learning saas considère que le jeu de données est propre. Et nettoyer le jeu de données c'est 90% du temps.
-  beaucoup de choses à apprendre

Deeplearning

Basé sur un réseau de neurones.

Deeplearning à la mode car les perf continue de grimper avec l'augmentation des données.

Inconvénient : il faut beaucoup de données.

C'est très coûteux en terme de calcul. Calcule matriciel et vectoriel : carte graphique.

C'est très complexe pour arriver à apprendre ce qu'on veut.

Convolution. Permet de réduire les info d'une image

Max pooling : prend la valeur max de la convolution.

Ces techniques permettent de réduire le nombre de calcul à faire. On enchaine des couches de convolution et de pooling sur notre réseau de neurones.

Pourquoi deeplearning ? C'est juste un réseau de neurones mais avec plus de couches. Avant on avait pas la puissance de calcul mais la logique existe depuis longtemps (Yann Lecun).

Framework : torche, caffe, tensorflow, dl4j en java. Keras : surcouche de tensorflow.

On peut réutiliser un réseau appris pour le modifier : transfert learning. Ou fine tuning

Style transfert. Appliquer une image de style sur une vrai image

Doodle. Permet de comprendre le style d'une image et de l'appliquer sur une image avec d'autre forme. Exemple des falaises d'etretat

Récurent neural network : ce qu'utilise Google pour translate

Renforcement learning : système d'apprentissage par reward à chaque action. Utilisé dans la robotique. Exemple des jeux Atari. C'est la techno qui a batu le joueur de go.
