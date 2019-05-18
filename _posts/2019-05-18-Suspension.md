---
Title: "Suspension"
layout: article
lang: FR
ref: post10
image: "http://wiki.walkingmachine.ca/images/e/e8/Suspension1.png 
---
## Suspension
Lors de la dernière RoboCup en 2018, S.A.R.A. a perdu tous ses points dans une épreuve puisqu’elle a eu des problèmes à franchir un cadre de porte, aussi banal que ça puisse sembler. Le petit dénivèlement du cadre de porte, franchi en diagonale, a fait en sorte que l’une des roues de cette dernière est restée en l’air pendant un moment, mais puisque S.A.R.A. n’a pas de capteur pour le savoir, elle a cru que cette roue la faisait tourner sur elle-même. Les données qui lui étaient fournies ne faisait donc plus vraiment de sens et elle ne parvenait plus à se situer dans l’espace. 
C’est un petit projet de mécanique, mais qui peut représenter un malgré tout un défi, puisque la suspension ne doit pas interférer avec la rigidité du châssis (Éviter que la tête oscille) et ne doit pas inutilement déstabiliser S.A.R.A ni modifier son système de locomotion. Le problème origine du fait que S.A.R.A. a quatre roues, et qu’il est impossible, pour un système rigide, d’avoir plus que trois points d’appui avec le sol. Plus spécifiquement, ce n’est pas une suspension en tant que tel que SARA doit avoir, mais plutôt un système mécanique qui permet à toutes les roues de rester en contact avec le sol afin d’éviter qu’une roue ne tourne dans le vide, une suspension étant une solution parmi d’autres.
C’est avec cet aspect en tête que l’équipe mécanique a développé un pivot entre les deux roues à l’arrière au lieu d’une suspension en tant que tel afin de simuler trois points (en triangle) d’appuis pour S.A.R.A. Puisque le centre de masse de S.A.R.A. était déjà plutôt à l’avant, elle n’est pas devenue instable à la suite de cet ajout.

![](http:// http://wiki.walkingmachine.ca/images/6/6f/Suspension2.png)

La « suspension » permet au robot de franchir de légers obstacles sans perdre le nord, et sans non plus se débalancer inutilement. Le système permet aussi au robot de se déplacer plus naturellement sur des planchers légèrement inégaux.
Cependant, le système, malgré sa simplicité et son coût très faible cause certains problèmes : les moteurs qui assurent le mouvement du robot à l’avant se déplacent par eux-mêmes en forçant contre la transmission lors des accélérations maximales et la transmission saute des dents d’engrenages puisque l’arbre des moteurs se déplacent. Le problème origine de la rigidité diminuée des supports à moteurs sur la plaque de base de S.A.R.A. à cause des espaceurs pour mettre à niveau l’avant avec l’arrière. 
L’équipe mécanique a maintenant un nouveau problème à corriger, mais S.A.R.A. va-t-elle garder son vieux système de locomotion encore longtemps?
