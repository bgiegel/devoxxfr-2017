# Mettre en place sa sécurité et sa gestion d'identité en 2017

- De plus en plus de gens utilisent leurs vrai identité sur Internet 
- Beaucoup de gens font encore l'authentification eux même. 
- Diy must die : pollution de code , Bad practices, pas d'économie d'échelle. 
- Différentes spec pour s'authentifier sur keycloak. 
  - Saml2 : XML énorme.. à éviter. 
  - Oauth 2. Framework. 
  - OpenID. Surcouche Oauth2.  Concept d'identité pas uniquement d'accès. Gestion de la session 
- Jwt: json web token. 3 partie. 
  - Loader : algo utiliser pour signature. 
  - Payload ou claims. Expiration, username, roles 
  - Signature. Encodage en base 64 
- Keycloak : open source 
- Adaptateur pour spring. Wildfly, node, générique... 
- Détection de brute force, rotation de clé. One Time password 
- Dans webinf ajouter fichier keycloak json pour la config du serveur
