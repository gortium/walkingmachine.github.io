---
Title: "Battery Management System (BMS)"
layout: article
lang: EN 
ref: post
---

## Battery Management System (BMS)

To be able to supervise our battery which has six cellules, of a total of 800wh, we are using a Battery Management System created by our members. We could have chosen an already made alternative, but, to simplify the communication with the card and because of the rarity of a solution adapted to our needs, we chose a learning optical and so to conceive our own.

We believe that a minimalist controller that has every functionality we want and allows us to develop fast is highly advantageous. In the past we used an Arduino with the Atmega328 to conceive our cards. The community surrounding this card is large and allow to highly accelerate the development of a program and transfer it to another programmer. Also, the Atmega328 allows a mode of low consumption interesting for a BMS.

After a phase of developing and debugging, our card reached a viable state, but not sufficiently satisfying. The protection of a lithium battery is difficult. Mistakes are not allowed, if the card faulty and over-uncharged the battery, it’s it death. If the card fails and a cellule’s tensions goes too low, the cellule will be dead.

To limit the risk of failure, our solution included two controllers Atmega to create a redundancy and extending the number of analogic lecture possible was eight by controllers. The two controllers communicate together to transfer the data to monitor it.

The more a system is complex the higher the risk of failure, at that moment the redundancy is useless, because it inverse this tendency.
