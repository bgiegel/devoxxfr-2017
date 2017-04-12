# Exécution de code : mais que se passe-t-il vraiment ?

Intéressant, mais long et en anglais et un peu fouillis.

Javap :

Décompilé en ligne de commande.

-c : affiche les commandes bytecode
-verbose : plus d'infos
200 byte code différent.. add, Sub, i2l (conversion).
Invokdynamic

- Écrire son bytecode : asm, bytebuddy

- JIT (juste un time)

Le but est d'optimiser le nombre de traitement à faire pour calculer un résultat

Type d'optimisation

- inlining

- Dead code élimination

- loop unrolling

- Locker coarsening

But : élimination des accès à la mémoire principal. Éviter les Locker,...

Voir : [simple 8bit assembler simulator](https://schweigi.github.io/assembler-simulator)

Démo exécution assembleur. Les processeurs aujourd'hui ne font plus ça. C'est bcp plus complexe. Il y a des notions de cache. Plusieurs coeurs.

Les cache partent du principes que les choses qui vont ensemble sont contiguës.. alors que si on parcours un liste de string il y a des pointeurs qui contienne des pointeurs... Rien n'est contigüe.

Le fait que le processeur tourne à 100% ne veut pas dire qu'on calcul le plus vite possible. Si il y a des miss dans le cache on va être obligé d'attendre que les donnees arrivent.
