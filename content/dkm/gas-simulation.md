---
date: 2025-12-14T13:20:57+01:00
title: Simulateur de gaz
source: http://source.st
cost: 2750
financed: 80
author: Hilaire Fernandes
version: "1.0"
apiVersion: "25.12"
---
Le modèle permet de définir une enceinte rectangulaire et un nombre
arbitraire de parois et d'atomes d'argon. Le modèle simule des **gaz
parfaits** et une interaction avec les parois par réflexion diffuse
ou des **gaz réels** avec à la fois l'interaction des parois et le
potentiel inter-atomique de Lennard-Jonnes.

Au cours de la simulation, la consigne de température de toutes les
parois, y compris l'enceinte, s'ajuste à la souris. Un nombre
arbitraire de sondes de température couvrant des zones rectangulaires
est également disponible.


```st
| figure |
figure := DrGeoFigure new.
figure segmentDe: 1@2 à: 5@3.
```





