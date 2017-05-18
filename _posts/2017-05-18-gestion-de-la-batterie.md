---
Title: "Gestion de la batterie (BMS)"
layout: article
lang: FR
ref: post
---

## Gestion de la batterie (BMS)

Afin de pouvoir surveiller notre batterie à six cellules, d’un total de 800wh, nous utilisons un Battery Management System créé par nos membres. Nous aurions pu choisir une alternative déjà fait, mais, afin de simplifier la communication avec la carte ainsi que par rareté de solution adapté à nos besoins, nous avons choisi une optique d’apprentissage et, ainsi, le concevoir nous-même.

Nous croyons qu’un contrôleur minimaliste qui possède toutes les fonctionnalités d’en nous désirons et qui nous permet un développement très rapide est grandement avantageux. Par le passé, nous avons utilisé un Arduino avec les Atmega328 pour concevoir nos cartes. En effet, la communauté autour de cette carte est très grande et permet d’accélérer grandement le développement d’un programme et le transfert de celui-ci à un autre programmeur. De plus, le Atmega328 permet un mode de basse consommation très intéressant pour un BMS.

Après plusieurs phases de développements et de débogages, notre carte a atteint un stade fiable, mais pas suffisamment satisfaisant. La protection d’une batterie au lithium est très difficile. L’erreur n’est pas permise, si la carte est défaillante et a le malheur de sur-décharger la batterie, c’est la mort de celle-ci. Si la carte tombe en panne et une des cellules a une tension trop basse, c’est la mort de la cellule.

Pour limiter les risques de plantage, notre solution inclus deux contrôleurs Atmega dans le but de créer une redondance tout en étendant le nombre de lecture analogique possible était de huit par contrôleur. Les deux contrôleurs communiquent ensemble pour transférer les données à des fin de monitorage.

Plus un système est complexe plus le risque de planter est élevé, c’est à ce moment que la redondance est utile, car elle inverse cette tendance.
