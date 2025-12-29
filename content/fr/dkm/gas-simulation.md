---
date: 2025-12-14T13:20:57+01:00
title: Simulateur de gaz
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

![Gas Simulation](dkm/gas-simulation.png#center)


```st
GasSimulation new
   fenceOrigin: 0@0 corner: 300@200;
   addWallFrom: 100@0 to: 80@85;
   addWallFrom: 100@200 to: 80@105;
   addMolecules: 50
```





