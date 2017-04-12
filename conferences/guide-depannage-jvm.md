# Le guide de dépannage de la jvm

Jinfo permet d'avoir les info de conf d'une instance de jvm

JPS. Permet de lister les process java uniquement

Quand on a une jvm bloquée :
- jstack PID
- Kill -3 : redirigé la sortie dans la stdout
- nommer les thread pour faciliter les analyses
