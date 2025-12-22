---
date: 2025-12-22
title: Gassimulator
source: http://source.st
status: "developed" # developed | project | progress | improvement
cost: 2750
financed: 80
author: Hilaire Fernandes
version: "1.0"
apiVersion: "25.12"
---
Das Modell ermöglicht es, ein rechteckiges Gehäuse und eine beliebige
Anzahl von Wänden und Argonatomen zu definieren. Das Modell simuliert
**ideale Gase** und eine Interaktion mit den Wänden durch diffuse
Reflexion oder **reale Gase** sowohl mit der Wandinteraktion als auch
mit dem Lennard-Jones-Interatomar-Potential.

Während der Simulation lässt sich der Temperatursollwert aller Wände,
einschließlich des Gehäuses, mit der Maus anpassen. Eine beliebige
Anzahl von Temperaturfühlern, die rechteckige Bereiche abdecken, ist
ebenfalls verfügbar.

![Gas Simulation](/dkm/gas-simulation.png#center)


```st
GasSimulation new
   fenceOrigin: 0@0 corner: 300@200;
   addWallFrom: 100@0 to: 80@85;
   addWallFrom: 100@200 to: 80@105;
   addMolecules: 50
```
