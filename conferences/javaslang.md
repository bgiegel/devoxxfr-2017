# Javaslang

Présentation d'une petite lib prometteuse permettant d'avoir les avantages de certains langages fonctionnels tel que Scala.

Java 8 quelques défauts :
- Quelque structures fonctionnelles
- Pas de tuples
- Optional pas serialisable ni iterable
- CheckedException

Javaslang vient pallier à ça

- Tuple très utile pour initier des maps
- Lazy : classe permettant d'initialiser à la première utilisation
- Either et try. Permet de se passer des bloc try catch en utilisant la programmation fonctionnel.
- Les collections sont immutable donc on peut faire des remove dessus.
- pattern matching + Either = plus de try catch.
