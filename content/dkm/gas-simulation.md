---
date: 2025-12-14T13:20:57+01:00
draft: false
title: Simulateur de gaz
cost: 2500
financed: 80
author: Hilaire Fernandes
version: 1.0
apiVersion: 25.12
---
Le modèle permet de définir une enceinte avec un nombre arbitraire de
parois et d'atomes d'argon. Le modèle simule des **gaz parfaits**,
sans potentiel inter-atomique, avec uniquement une interaction avec
les parois par réflexion diffuse ou des **gaz réels** avec à la fois
l'interaction avec les parois et le potentiel inter-atomique --
potentiel de Lennard-Jonnes.

Au cours de la simulation, la consigne de température de toutes les
parois, y compris l'enceinte, s'ajuste à la souris. Un nombre
arbitraire de sondes de température couvrant des zones rectangulaires
est également disponible.


```st
| figure |
figure := DrGeoFigure new.
figure segmentDe: 1@2 à: 5@3.
```





