## TP1 – Programmation Java Avancé
# Objectif :
Ce TP a pour objectif de mettre en pratique les classes Java, les interfaces Comparable et Comparator, les exceptions ainsi que les collections HashSet, TreeSet et TreeMap.

---
# Exercice 1 : Classe Livre

-	Création de la classe Livre. 
-	Ajout des attributs : titre, auteur, prix et nombre de pages. 
-	Création des constructeurs, getters et setters. 
-	Utilisation de afficheToi(), toString(), equals() et hashCode(). 
-	Test de la classe dans TestLivre.

  
  ---
![demo](https://github.com/salmaly-ui/Tp1JavaAv/blob/main/Exercice1.jpg?raw=true)
La classe Livre fonctionne correctement et les informations des livres sont affichées dans la console.
# Pourquoi hashCode() ?
HashSet utilise hashCode() avec equals() pour reconnaître les doublons.
# Exercice 2 : Tri des livres
a) Avec Comparable
La classe Livre implémente Comparable<Livre>. Les livres sont triés selon l'auteur puis selon le titre.
![demo](https://github.com/salmaly-ui/Tp1JavaAv/blob/main/Ex2a.jpg?raw=true)
Le tableau de livres est correctement trié.
b) Avec Comparator
Un Comparator<Livre> est utilisé pour définir le tri sans modifier la règle de comparaison principale de la classe
![demo](https://github.com/salmaly-ui/Tp1JavaAv/blob/main/Ex2b.jpg?raw=true)
Le tri est également effectué correctement.
# Exercice 3 : Classe Etagere

Une classe Etagere est créée avec une capacité limitée.
Deux exceptions sont utilisées :
-EtagerePleineException lorsque l'étagère est pleine. 
-EtagereVideException lorsque l'étagère est vide

![demo](https://github.com/salmaly-ui/Tp1JavaAv/blob/main/Ex3.jpg?raw=true)
L'ajout, la recherche et l'accès aux livres fonctionnent correctement et l'exception est déclenchée lorsque l'étagère est pleine.

---
# Exercice 4 : Collections

1. HashSet
Le HashSet utilise equals() et hashCode() pour déterminer si deux livres sont identiques. Dans notre cas, deux livres ayant le même titre et le même prix sont considérés comme égaux.
![demo](https://github.com/salmaly-ui/Tp1JavaAv/blob/main/Ex4_1.jpg?raw=true)
---
2. TreeSet
Le TreeSet utilise une comparaison pour organiser les livres selon leur prix.
Remarque : si deux livres ont le même prix et que le comparateur retourne 0, le TreeSet peut considérer ces deux livres comme identiques.

![demo](https://github.com/salmaly-ui/Tp1JavaAv/blob/main/Ex4_2.jpg?raw=true)
---
4. TreeMap
Le TreeMap permet d'associer chaque livre à son nombre de pages. Les livres sont organisés selon leur prix.
![demo](https://github.com/salmaly-ui/Tp1JavaAv/blob/main/Ex4_3.jpg?raw=true)
---

Conclusion
Ce TP nous a permis de pratiquer les génériques et les collections Java, ainsi que le tri avec Comparable et Comparator. Nous avons également appris à utiliser les exceptions et les collections HashSet, TreeSet et TreeMap.

