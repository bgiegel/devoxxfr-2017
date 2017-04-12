# Migrer à jigsaw : En douleur ou en douceur ?

Jdeps : voir les dépendances de l'application

Unamned module : quand on fait pas de module java met tout dans ce module de base

On peut ouvrir des modules directement dans la commande java avec add-opens. Même chose pour l'export avec add-exports

--> très fastidieux

On peut à présent utiliser l'option : permit-illegal-access

Ensuite l'objectif c'est d'avoir une appli java9 pas 8. Donc on peut créer un module. On va déclarer les module dont on dépend avec require.

Ça empêche pas de devoir remettre les add-opens mais là on va pouvoir limiter l'ouverture au module vertx qui l'utilise.

Conclusion

Plutôt douleur pour l'instant pour la transition java9. Beaucoup de changement. Le permit-illegal-access va permettre de faire une migration en douceur pour éviter l'effet Big Bang.
