# Optimiser les performances d'une webapp

Plus de personnes naviguent sur mobile que sur desktop

Pk pages sont longues ?

Elle contiennent beaucoup de data

3/4 des sites mettent plus de 10s à charger sur mobile.

Comment faire pour améliorer les performances ?

1. mesurer

Loadtime et First paint

Webpagetest, pagespeed

Chrome : outil pour simuler une 3G

2. transport

Mettre script à la fin du body pas dans le head

Http2 pas activé par défaut dans les containers.

3. Limiter

Minification des ressources.

Des DTO qui collent à l'API

Compression du texte

Bootstrap et founders on un coups...

Les framework sont aujourd'hui tous modulaires.

UnCSS. Généré un CSS épurée.

Compression avec imagemin

Balise picture pour utiliser des images avec format différent comme webp et autre paramètre.

Fonts : pas la même taille. Éviter font svg. Voir woff2.

JS: treeshaking. Serverside rendering. Modules. Etc...

4. Cache

E-tag permet de mettre un gros maxage et de toujours rafraîchir la page si il y a un changement en rajoutant un md5 différent à chaque changement.

5. Offline

Service workers : permet de lancer des traitements dans d'autres thread.

Communique entre eux par échange de messages.

6. Anticiper

Preload

Prefetch : Si tu as du temps télécharge cette ressource.

First do it
Then do it right.
Then do it better.
